# JRR Personal Blog

A personal blog built with Jekyll for GitHub Pages, featuring a blog, gratitude diary, and daily journal.

## 🌟 Features

- **Blog**: Share your thoughts, experiences, and learnings
- **Gratitude Diary**: Daily practice of documenting things you're grateful for
- **Daily Journal**: Reflect on your day, track progress, and set intentions
- **Responsive Design**: Clean, mobile-friendly interface
- **Easy to Use**: Markdown-based content with simple templates

## 🚀 Getting Started

### Enable GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select your main branch
4. Click "Save"
5. Your site will be available at `https://[username].github.io/[repository-name]/`

### Local Development

To run the site locally:

```bash
# Install Jekyll (if not already installed)
gem install bundler jekyll

# Create a Gemfile in your project root
echo 'source "https://rubygems.org"
gem "github-pages", group: :jekyll_plugins
gem "webrick"' > Gemfile

# Install dependencies
bundle install

# Run the site locally
bundle exec jekyll serve

# Visit http://localhost:4000 in your browser
```

## 📝 Creating Content

### Blog Posts

Create a new file in `_posts` folder with the format: `YYYY-MM-DD-title.md`

```markdown
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD
author: Your Name
tags: [tag1, tag2]
---

Your content here...
```

### Gratitude Entries

Create a new file in `_gratitude` folder with the format: `YYYY-MM-DD-title.md`

See the [gratitude template](/templates/gratitude-template) for a complete example.

```markdown
---
layout: gratitude
title: "Gratitude - [Date]"
date: YYYY-MM-DD
mood: [happy/content/peaceful/energetic/reflective]
grateful_for:
  - "Thing 1"
  - "Thing 2"
  - "Thing 3"
---

Your reflection here...
```

### Journal Entries

Create a new file in `_journal` folder with the format: `YYYY-MM-DD-title.md`

See the [journal template](/templates/journal-template) for a complete example.

```markdown
---
layout: journal
title: "Journal - [Date]"
date: YYYY-MM-DD
highlights:
  - "Positive moment 1"
  - "Positive moment 2"
challenges:
  - "Challenge 1"
lessons_learned:
  - "Lesson 1"
tomorrow_goals:
  - "Goal 1"
---

Your journal entry here...
```

## 📁 Project Structure

```
.
├── _config.yml           # Jekyll configuration
├── _layouts/             # Page layouts
│   ├── default.html      # Base layout
│   ├── post.html         # Blog post layout
│   ├── gratitude.html    # Gratitude entry layout
│   └── journal.html      # Journal entry layout
├── _posts/               # Blog posts
├── _gratitude/           # Gratitude diary entries
├── _journal/             # Daily journal entries
├── templates/            # Templates for new entries
│   ├── gratitude-template.md
│   └── journal-template.md
├── assets/
│   └── css/
│       └── style.css     # Custom styles
├── index.md              # Homepage
├── blog.md               # Blog listing page
├── gratitude.md          # Gratitude listing page
├── journal.md            # Journal listing page
└── about.md              # About page
```

## 🎨 Customization

### Site Settings

Edit `_config.yml` to customize:
- Site title and description
- Author information
- Email address

### Styling

Edit `assets/css/style.css` to customize the appearance of your site.

## 📚 Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## 📄 License

This project is licensed under the GNU General Public License v3.0 - see the LICENSE file for details.
