# GitHub Profile README Setup Guide

This repository contains a dynamic GitHub profile README that automatically updates with your latest stats, quotes, and activity.

## 🚀 Quick Setup

1. **Fork or copy this repository** to a new repository named exactly as your GitHub username
   - Example: If your username is `johndoe`, create a repository named `johndoe`

2. **Enable GitHub Actions** in your repository settings

3. **Update the README.md** with your personal information:
   - Replace contact links in the "Connect with Me" section
   - Update the "About Me" section with your details
   - Customize the tech stack badges to match your skills

4. **Set up repository secrets** (optional but recommended):
   - `WAKATIME_API_KEY`: For coding time tracking (get from [WakaTime](https://wakatime.com/settings/account))
   - `GH_TOKEN`: Personal access token for enhanced GitHub stats

## 🔧 Configuration

### Personal Information
Edit these sections in `README.md`:
- Contact information (email, LinkedIn, Twitter, portfolio)
- About Me section
- Tech stack badges

### GitHub Actions
The profile automatically updates using two workflows:

#### 1. `update-readme.yml` (Daily at 6 AM UTC)
- Updates GitHub stats
- Refreshes daily motivational quote
- Updates last modified date
- Updates recent project repositories

#### 2. `wakatime-stats.yml` (Daily at 7 AM UTC) - Optional
- Updates coding time statistics
- Requires WakaTime API key

### Customization Options

#### Tech Stack Badges
Update the badges in the "Tech Stack" section to reflect your skills:
```markdown
![Your-Tech](https://img.shields.io/badge/Your--Tech-color?style=for-the-badge&logo=logo-name&logoColor=white)
```

#### Themes
The profile uses `tokyonight` theme. You can change to other themes:
- `dark`
- `radical` 
- `merko`
- `gruvbox`
- `vue-dark`

Replace `theme=tokyonight` in the URLs with your preferred theme.

#### Profile Stats Services Used
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [GitHub Readme Streak Stats](https://github.com/DenverCoder1/github-readme-streak-stats)
- [GitHub Profile Trophy](https://github.com/ryo-ma/github-profile-trophy)
- [GitHub Readme Activity Graph](https://github.com/Ashutosh00710/github-readme-activity-graph)
- [Shields.io](https://shields.io/) for badges
- [readme-typing-svg](https://github.com/DenverCoder1/readme-typing-svg) for animated text

## 🎯 Optional Enhancements

### WakaTime Integration
1. Sign up at [WakaTime](https://wakatime.com/)
2. Install WakaTime plugin in your code editor
3. Get your API key from WakaTime settings
4. Add `WAKATIME_API_KEY` to repository secrets

### Enhanced GitHub Token
1. Create a personal access token with `repo` and `user` permissions
2. Add `GH_TOKEN` to repository secrets for enhanced stats

### Profile Views Counter
The profile includes a view counter that automatically tracks visitors.

## 🔄 Manual Updates

You can manually trigger updates by:
1. Going to Actions tab in your repository
2. Selecting "Update README Profile" workflow
3. Clicking "Run workflow"

## 🎨 Advanced Customization

### Custom Quotes
Edit the quotes array in `.github/workflows/update-readme.yml` to add your favorite quotes.

### Additional Stats
You can add more sections like:
- Top languages
- Recent blog posts (if you have a blog with RSS)
- Recent GitHub activity
- Spotify playing status

### Styling
The profile uses HTML and CSS for advanced styling. You can customize:
- Colors and themes
- Layout and alignment
- Fonts and sizing
- Animations and effects

## 📋 Troubleshooting

### Common Issues
1. **README not updating**: Check if GitHub Actions are enabled
2. **Stats not showing**: Verify repository name matches your username exactly
3. **WakaTime not working**: Ensure API key is correctly set in secrets

### Support
- Check the [GitHub Community](https://github.community/) for general GitHub questions
- Review individual service documentation for specific integrations

## 📄 License

This template is open source and available under the MIT License.