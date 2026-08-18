# 🎉 Welcome to SocOps Bingo!

Welcome to your local development environment! Here's a quick tour to get you up to speed.

## 🚀 What's Running Now

✅ **Dev Server** is live at `http://localhost:5166`  
✅ **.NET 10 SDK** verified (v10.0.302)  
✅ **Project built** and ready to go  

## 📁 Project Structure at a Glance

```
SocOps/
├── Components/          → Blazor UI components (BingoBoard, BingoSquare, etc.)
├── Pages/               → Routable pages (Home, Counter, Weather, etc.)
├── Services/            → Game logic (BingoGameService, BingoLogicService)
├── Models/              → Data models (GameState, BingoLine, etc.)
├── Data/                → Questions database
├── Layout/              → App layout & navigation
└── wwwroot/             → Static assets (CSS, JavaScript, images)
```

## 🎮 Key Features

- **BingoBoard** - The main game grid component
- **GameScreen** - Active gameplay experience
- **StartScreen** - Game initialization and setup
- **BingoGameService** - Manages game state and logic

## 💻 Development Commands

```bash
# Build the project
dotnet build SocOps/SocOps.csproj

# Run dev server (already running!)
dotnet run --project SocOps/SocOps.csproj

# The app will be available at: http://localhost:5166
```

## 🔧 Next Steps

1. **Explore the Components** - Start with `BingoBoard.razor` and `GameScreen.razor`
2. **Review Game Logic** - Check `BingoLogicService.cs` for the core game mechanics
3. **Add Content** - Modify questions in `Data/Questions.cs`
4. **Style & Polish** - Update CSS in `wwwroot/css/app.css`

## 📚 Workshop Materials

Complete learning materials are available in the `workshop/` folder:
- `00-overview.md` - Project overview
- `01-setup.md` - Setup instructions
- `02-design.md` - Design patterns & architecture
- `03-quiz-master.md` - Game mechanics guide
- `04-multi-agent.md` - Advanced topics
- `05-complete.md` - Completion checklist

Available in: English, Spanish (`es/`), and Portuguese (`pt_BR/`)

## 🌐 Your Dev Environment is Ready!

The site should now be open in your browser. Start building! 🚀

**Need help?** Check the main [README.md](README.md) for full documentation.
