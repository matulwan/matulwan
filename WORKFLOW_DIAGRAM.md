# 🔄 Snake Animation Workflow Diagram

## How the Snake Game Works

```
┌─────────────────────────────────────────────────────────────────┐
│                     GITHUB PROFILE WORKFLOW                      │
└─────────────────────────────────────────────────────────────────┘

┌─────────────────┐
│  You Push Code  │
│   to GitHub     │
└────────┬────────┘
         │
         ▼
┌─────────────────────────────────────────────────────────────────┐
│                    TRIGGERS (Any of these)                       │
├─────────────────────────────────────────────────────────────────┤
│  1. Push to main branch                                         │
│  2. Every 24 hours (automatic)                                  │
│  3. Manual trigger (Actions tab)                                │
└────────┬────────────────────────────────────────────────────────┘
         │
         ▼
┌─────────────────────────────────────────────────────────────────┐
│              GITHUB ACTIONS WORKFLOW STARTS                      │
│                  (.github/workflows/snake.yml)                   │
└────────┬────────────────────────────────────────────────────────┘
         │
         ▼
┌─────────────────────────────────────────────────────────────────┐
│                    STEP 1: SETUP                                 │
│  • Spin up Ubuntu virtual machine                               │
│  • Install required dependencies                                │
│  • Authenticate with GitHub token                               │
└────────┬────────────────────────────────────────────────────────┘
         │
         ▼
┌─────────────────────────────────────────────────────────────────┐
│              STEP 2: FETCH CONTRIBUTION DATA                     │
│  • Read your GitHub contribution graph                          │
│  • Get all commits, PRs, issues from past year                  │
│  • Organize data by date and intensity                          │
└────────┬────────────────────────────────────────────────────────┘
         │
         ▼
┌─────────────────────────────────────────────────────────────────┐
│              STEP 3: GENERATE SNAKE ANIMATION                    │
│  • Create snake path through contributions                      │
│  • Snake "eats" contributions chronologically                   │
│  • Generate SVG animation frames                                │
│  • Create light theme version                                   │
│  • Create dark theme version                                    │
└────────┬────────────────────────────────────────────────────────┘
         │
         ▼
┌─────────────────────────────────────────────────────────────────┐
│                STEP 4: SAVE TO OUTPUT BRANCH                     │
│  • Create/update 'output' branch                                │
│  • Save: github-contribution-grid-snake.svg (light)             │
│  • Save: github-contribution-grid-snake-dark.svg (dark)         │
│  • Commit and push to output branch                             │
└────────┬────────────────────────────────────────────────────────┘
         │
         ▼
┌─────────────────────────────────────────────────────────────────┐
│                   WORKFLOW COMPLETE ✅                           │
│  • Animation files are now in 'output' branch                   │
│  • README.md references these files                             │
│  • Snake appears on your profile!                               │
└─────────────────────────────────────────────────────────────────┘
         │
         ▼
┌─────────────────────────────────────────────────────────────────┐
│                  VISITOR VIEWS YOUR PROFILE                      │
│  • GitHub loads README.md                                       │
│  • Fetches snake SVG from output branch                         │
│  • Displays animated snake eating contributions                │
│  • Auto-selects light/dark theme based on user preference      │
└─────────────────────────────────────────────────────────────────┘
```

## 📊 Data Flow

```
Your GitHub Activity
       ↓
Contribution Graph
       ↓
GitHub Actions Workflow
       ↓
Snake Animation Generator
       ↓
SVG Files (Light + Dark)
       ↓
Output Branch
       ↓
README.md Display
       ↓
Your Profile Visitors See It!
```

## 🎯 File Locations

```
Repository Structure:

matulwan/                          (main branch)
├── README.md                      ← References snake SVGs
├── .github/workflows/snake.yml    ← Workflow definition
└── ...

matulwan/                          (output branch)
├── github-contribution-grid-snake.svg       ← Light theme
└── github-contribution-grid-snake-dark.svg  ← Dark theme
```

## ⏱️ Timeline

```
Day 1 (Setup):
00:00 - Push code to GitHub
00:01 - Workflow triggers automatically
00:02 - Snake animation generated
00:03 - Files saved to output branch
00:04 - Profile updated with snake! ✅

Day 2 (Auto-update):
00:00 - Scheduled workflow runs
00:01 - Fetches new contributions
00:02 - Updates snake animation
00:03 - Profile refreshed automatically

Every Day After:
- Automatic updates at midnight UTC
- Snake grows with your contributions
- No manual intervention needed
```

## 🔄 Update Cycle

```
┌──────────────────────────────────────────────────┐
│                                                  │
│  Make Commits → Workflow Runs → Snake Updates   │
│       ↑                                    ↓     │
│       └────────── 24 Hours Later ──────────┘     │
│                                                  │
└──────────────────────────────────────────────────┘
```

## 🎨 Theme Selection Logic

```
Visitor Opens Your Profile
         ↓
    ┌────┴────┐
    │         │
Dark Mode?  Light Mode?
    │         │
    ▼         ▼
 snake-dark  snake-light
    │         │
    └────┬────┘
         ▼
   Displays Snake
```

## 🛠️ Technical Stack

```
┌─────────────────────────────────────────────┐
│           Technology Stack                   │
├─────────────────────────────────────────────┤
│  • GitHub Actions (CI/CD)                   │
│  • Platane/snk (Snake generator)            │
│  • SVG (Animation format)                   │
│  • GitHub API (Data source)                 │
│  • Ubuntu VM (Runtime environment)          │
│  • Git (Version control)                    │
└─────────────────────────────────────────────┘
```

## 🔐 Permissions Flow

```
GitHub Actions Workflow
         ↓
Uses GITHUB_TOKEN
         ↓
    ┌────┴────┐
    │         │
Read Repo   Write Output
    │         │
    ▼         ▼
Get Data   Save SVGs
```

## 📈 Contribution Processing

```
Raw GitHub Data:
┌───┬───┬───┬───┬───┬───┬───┐
│ 0 │ 3 │ 5 │ 2 │ 8 │ 1 │ 4 │  (Commits per day)
└───┴───┴───┴───┴───┴───┴───┘
         ↓
Snake Algorithm:
         ↓
Animated Path:
  🐍 → → → → → → → → → →
         ↓
Final SVG:
  [Animated snake eating contributions]
```

## 🎬 Animation Frames

```
Frame 1:  🐍 · · · · · ·
Frame 2:  · 🐍 · · · · ·
Frame 3:  · · 🐍 · · · ·
Frame 4:  · · · 🐍 · · ·
Frame 5:  · · · · 🐍 · ·
Frame 6:  · · · · · 🐍 ·
Frame 7:  · · · · · · 🐍
         (Loops continuously)
```

## 🚀 Performance

```
Workflow Execution Time:
├── Setup: ~30 seconds
├── Data Fetch: ~20 seconds
├── Generate Animation: ~40 seconds
├── Save to Branch: ~10 seconds
└── Total: ~2 minutes ✅

File Sizes:
├── snake.svg (light): ~50-100 KB
└── snake-dark.svg: ~50-100 KB

Load Time on Profile:
└── < 1 second (cached by GitHub)
```

## 🔍 Debugging Flow

```
Something Wrong?
       ↓
Check Actions Tab
       ↓
   ┌────┴────┐
   │         │
Success?   Failed?
   │         │
   ▼         ▼
Check     Read Error
Output    Message
Branch       ↓
   │      Fix Issue
   │         ↓
   └─→ Re-run Workflow
```

## 💡 Key Points

1. **Automatic**: Runs without manual intervention
2. **Reliable**: Uses GitHub's infrastructure
3. **Fast**: Completes in ~2 minutes
4. **Efficient**: Only updates when needed
5. **Scalable**: Works with any contribution level
6. **Themed**: Adapts to user's preference

---

**This workflow ensures your snake is always up-to-date! 🐍✨**
