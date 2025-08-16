# DoneList User Stories

This repository contains dynamic user stories for the DoneList iOS app.

## Purpose

This repository serves as a content delivery system for DoneList's User Stories feature. The app fetches user stories from this repository to display community stories and motivational content to users.

## File Structure

- `user-stories.json` - Contains the user stories data in JSON format
- `README.md` - This file

## JSON Format

The `user-stories.json` file contains an array of user stories with the following structure:

```json
{
  "stories": [
    {
      "id": "unique_id",
      "title": "Story Title",
      "summary": "Brief summary of the story",
      "content": "Full story content with line breaks",
      "category": "story_category",
      "date": "YYYY-MM-DD"
    }
  ],
  "lastUpdated": "YYYY-MM-DD",
  "version": "1.0"
}
```

## Raw URL

The app fetches content from:
https://raw.githubusercontent.com/evendev1231/DoneList-UserStories/main/user-stories.json

## Updating Stories

To update user stories:

1. Edit the `user-stories.json` file
2. Commit and push changes:
   ```bash
   git add user-stories.json
   git commit -m "Update user stories with new content"
   git push origin main
   ```
3. The app will automatically fetch the updated content on next launch

## Categories

- `productivity` - Productivity and efficiency stories
- `motivation` - Motivation and inspiration stories  
- `habits` - Habit formation and behavior change stories

## Notes

- This repository is public to allow the app to fetch content without authentication
- Only user stories content is stored here, no app code or sensitive data
- Updates are reflected in the app within 24 hours (depending on app usage)
