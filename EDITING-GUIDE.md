# 📝 How to Edit Your Portfolio Website

## 🎯 Quick Start

**To update ANY content on your website, you only need to edit ONE file:**

👉 **`/src/app/data/portfolio-data.ts`**

That's it! This file contains everything - your name, projects, skills, about section, and social links.

---

## 🚀 How to Make Changes

### Step 1: Open the Data File
Navigate to `/src/app/data/portfolio-data.ts` in your code editor.

### Step 2: Edit the Content
Find the section you want to change and edit the text between the quotes `""`.

**Example:**
```typescript
name: "Leila Alswayan",  // ← Change your name here
```

### Step 3: Save & Refresh
- Save the file (Ctrl+S or Cmd+S)
- Refresh your browser to see the changes

---

## 📚 What You Can Edit

### 1. Personal Information
```typescript
name: "Your Name",
tagline: "Your Professional Title",
bio: "Your short bio",
```

### 2. Social Links
```typescript
social: {
  email: "your@email.com",
  github: "https://github.com/yourusername",
  linkedin: "https://linkedin.com/in/yourusername",
  // ... etc
}
```

### 3. Projects
Each project has:
- **title**: Project name
- **description**: Short summary (shows on cards)
- **detailedDescription**: Full description (shows on project page)
- **features**: List of features (bullet points)
- **technologies**: Tech stack used
- **images**: Array of image URLs
- **liveUrl**: Link to live project
- **githubUrl**: Link to GitHub repo

**To add a new project:**
1. Copy an entire project block (from `{` to `}`)
2. Paste it after the last project
3. Update the `id` to be unique
4. Edit all the content
5. Don't forget the comma after each project!

### 4. Skills
```typescript
skills: [
  { name: "Skill Name", level: 95, icon: "🎨" },
  // level is 0-100
]
```

### 5. About Section
```typescript
about: {
  intro: "Your introduction text",
  points: [
    "Point 1",
    "Point 2",
    // Add more points as needed
  ]
}
```

---

## ⚠️ Important Tips

### ✅ DO:
- Keep quotes around text: `"like this"`
- Keep commas at the end of lines: `name: "Text",`
- Save the file after making changes
- Use unique IDs for projects (1, 2, 3, etc.)

### ❌ DON'T:
- Remove quotes or commas
- Delete the structure (brackets, colons, etc.)
- Change the field names (like `name:`, `title:`, etc.)

---

## 🎨 Adding Images to Projects

You can add images in two ways:

### Option 1: Use Image URLs
```typescript
images: [
  "https://example.com/image1.png",
  "https://example.com/image2.png"
]
```

### Option 2: Leave Empty
```typescript
images: []
```

---

## 🆘 Troubleshooting

### Website not updating?
1. Make sure you saved the file
2. Hard refresh your browser (Ctrl+Shift+R or Cmd+Shift+R)
3. Check for any missing commas or quotes

### Syntax error?
- Look for missing commas
- Make sure all quotes are closed: `"text"`
- Check that brackets are balanced: `{...}`

---

## 💡 Pro Tips

1. **Test one change at a time** - Make small edits and refresh to see results
2. **Keep a backup** - Copy the file before making major changes
3. **Use the comments** - The file has helpful comments (lines starting with `//`)
4. **Copy & paste** - When adding items, copy existing ones to maintain the format

---

## 🎉 That's It!

You now have complete control over your portfolio content. No need to touch any other files - everything you need is in `portfolio-data.ts`!

Happy editing! ✨
