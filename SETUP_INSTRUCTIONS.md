# Quick Setup Instructions

## Step 1: Create GitHub Labels

Go to your repository and create these labels to enable proper filtering:

1. **Visit**: https://github.com/delwinbest/mysailinglog-feedback/labels
2. **Click**: "New label" button
3. **Create these labels**:

### Essential Labels
- **bug** (Red #d63031) - Something isn't working
- **feature-request** (Green #00b894) - New functionality  
- **needs-triage** (Yellow #f9ca24) - New issue awaiting review
- **in-progress** (Purple #6c5ce7) - Currently being worked on
- **triaged** (Green #00b894) - Reviewed and approved for development

### Priority Labels (Optional)
- **priority-critical** (Red #d63031)
- **priority-high** (Pink #e84393) 
- **priority-medium** (Blue #0984e3)
- **priority-low** (Green #00b894)

## Step 2: Test the Setup

1. Create a test issue using the "Bug Report" template
2. Create a test issue using the "Feature Request" template
3. Verify that labels are automatically applied
4. Check that the embed widgets work correctly

## Step 3: Update Embed URLs (Optional)

Once labels are created, you can update the embed URLs to filter by specific labels:

### For Feature Requests Only:
```
https://github.com/delwinbest/mysailinglog-feedback/issues?q=is%3Aissue+is%3Aopen+label%3Afeature-request+sort%3Aupdated-desc
```

### For Bugs Only:
```
https://github.com/delwinbest/mysailinglog-feedback/issues?q=is%3Aissue+is%3Aopen+label%3Abug+sort%3Aupdated-desc
```

## Current Status

✅ Repository created  
✅ Issue templates created  
✅ Application pages created  
⏳ Labels need to be created manually  
⏳ Project board setup (optional)

## Need Help?

If you encounter any issues, create an issue in this repository or contact the development team.