# SocOps Agent Instructions

**SocOps** is a Social Bingo game built with Blazor WebAssembly (.NET 10). Players find people matching questions to mark 5×5 grid squares and win with 5 in a row. Dev server: `http://localhost:5166`

## 🚀 MANDATORY Pre-Commit Checklist

```bash
dotnet build SocOps/SocOps.csproj
dotnet run --project SocOps/SocOps.csproj
# Manual test at http://localhost:5166
```

Before every commit:
- ✅ **Lint**: C# conventions (PascalCase public members), no unused imports/variables
- ✅ **Build**: `dotnet build` passes with no errors
- ✅ **Test**: Manually verify at http://localhost:5166; new game logic requires unit tests

## Project Structure

- **Components/**: Razor UI (BingoBoard, BingoSquare, GameScreen, StartScreen)
- **Services/**: BingoGameService (state + persistence), BingoLogicService (win detection)
- **Models/**: GameState, BingoLine, BingoSquareData
- **Data/**: Questions.cs (static question pool)
- **wwwroot/css/**: Custom utility classes (`.flex`, `.grid`, `.bg-accent`, etc.)

## Architecture

**State Management**: BingoGameService manages game state, persists to localStorage, raises `OnStateChanged` event. Components subscribe and re-render automatically.

**Component Hierarchy**: App → MainLayout → @Body → StartScreen/GameScreen → BingoBoard → BingoSquare (×25)

**Data Flow**: User action → Component calls BingoGameService method → Service updates state & fires event → Subscribers re-render → localStorage persists

## Styling & Design

- **CSS Utilities**: Custom classes in `wwwroot/css/app.css` (`.flex`, `.grid`, `.bg-accent`, `.text-*`, `.p-*`, `.rounded`, etc.)
- See `.github/instructions/css-utilities.instructions.md` for full reference
- **Design**: Avoid "AI slop" — choose distinctive fonts, bold accents, depth with gradients, context-specific aesthetics
- See `.github/instructions/frontend-design.instructions.md` for detailed guidance

## Component Development

**Adding a component**: Create `.razor` file in `SocOps/Components/`, use `[Parameter]` for props, subscribe to `GameService.OnStateChanged` in `OnInitialized()`, style with CSS utilities.

## Game Logic

**BingoLogicService**: Win detection (5 in a row horizontal/vertical/diagonal), question randomization, square marking.

**Questions**: Stored in `Data/Questions.cs` as static list. Keep questions engaging, diverse (interests, experiences, icebreakers), and not too specific to allow multiple valid matches.

## Resources

- [README.md](../README.md) — Main documentation
- [workshop/GUIDE.md](../workshop/GUIDE.md) — Learning materials
- [.github/instructions/css-utilities.instructions.md](.github/instructions/css-utilities.instructions.md) — CSS reference
- [.github/instructions/frontend-design.instructions.md](.github/instructions/frontend-design.instructions.md) — Design guide

---

**Keep the game fun and engaging!** 🎉
