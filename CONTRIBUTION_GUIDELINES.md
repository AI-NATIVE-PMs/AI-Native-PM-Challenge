# Contribution Guidelines: AI-Native PM Challenge Elite

![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Focus](https://img.shields.io/badge/Focus-Africa-orange)
![Level](https://img.shields.io/badge/Level-Elite-blue)

Welcome to the AI-Native PM Challenge Elite community. This guide explains how to contribute your work, share knowledge, and help others become AI-Native architects.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Submitting Your Weekly Work](#submitting-your-weekly-work)
3. [Code of Conduct](#code-of-conduct)
4. [Pull Request Process](#pull-request-process)
5. [Documentation Standards](#documentation-standards)
6. [Sunday Review Sessions](#sunday-review-sessions)
7. [Sharing Knowledge](#sharing-knowledge)
8. [Feedback & Reviews](#feedback--reviews)

---

## Getting Started

### Step 1: Fork the Repository

1. Go to [ai-native-pm-challenge](https://github.com/your-org/ai-native-pm-challenge)
2. Click the "Fork" button in the top-right corner
3. This creates your own copy of the repository

### Step 2: Clone Your Fork

```bash
git clone https://github.com/your-username/ai-native-pm-challenge.git
cd ai-native-pm-challenge
```

### Step 3: Create Your Participant Folder

```bash
mkdir -p participants/your-name
cd participants/your-name
touch README.md
```

### Step 4: Add Your Introduction

Create `participants/your-name/README.md`:

```markdown
# [Your Name]

## About Me
- **Location**: [City, Country]
- **Background**: [Your PM/tech background]
- **Goals**: [What you want to achieve]
- **Email**: [Your Email Address]
- **LinkedIn**: [Your profile]
- **GitHub**: [Your profile]

## Challenge Progress
- Week 1: [Status]
- Week 2: [Status]
- ... (will update as you progress)

## Key Learnings
[You'll update this as you go]
```

### Step 5: Commit and Push

```bash
git add .
git commit -m "Add participant: [Your Name]"
git push origin main
```

### Step 6: Submit a Pull Request

1. Go to the original repository
2. Click "Pull Requests" → "New Pull Request"
3. Select your fork and branch
4. Add a title: "Add participant: [Your Name]"
5. Submit!

---

## Submitting Your Weekly Work

### Folder Structure

```
participants/your-name/
├── README.md                    # Your intro
├── week-1/
│   ├── README.md                # Week 1 summary
│   ├── system-prompt.md         # Your PRD generator
│   ├── live-url.txt             # Deployed app link
│   └── learnings.md             # Key takeaways
├── week-2/
│   ├── README.md
│   ├── ui-demo.md
│   ├── live-url.txt
│   └── learnings.md
└── ... (weeks 3-12)
```

### What to Include in Each Week's README

**Minimum Requirements**:

```markdown
# Week [X]: [Challenge Name]

## Challenge Summary
[1-2 sentence description of what you built]

## Live URL
[Link to your deployed application]

## GitHub Repository
[Link to your code repository]

## Key Metrics
- [Metric 1]: [Value]
- [Metric 2]: [Value]
- [Metric 3]: [Value]

## What I Built
[Detailed description of your solution]

## Challenges & Solutions
1. **Challenge**: [What went wrong]
   **Solution**: [How you fixed it]

## Key Learnings
[3-5 main takeaways from this week]

## Next Steps
[What you'll improve next week]
```

### Bonus Content (Highly Encouraged)

- **Video Walkthrough**: Record a 3-5 minute Loom video
- **Code Highlights**: Interesting code snippets with explanations
- **Error Analysis**: What failed and why
- **Competitive Analysis**: How your solution compares
- **Business Model**: Pricing and unit economics
- **User Testimonials**: Quotes from real users

### Submitting Your Weekly Work

1. Create a folder: `participants/your-name/week-X/`
2. Add all required files
3. Commit and push:
   ```bash
   git add participants/your-name/week-X/
   git commit -m "Add Week X submission: [Your Name]"
   git push origin main
   ```
4. Submit a pull request with:
   - Title: "Week X Submission: [Your Name]"
   - Description: Link to your live URL and key metrics
   - Checklist: Confirm all required files are included

### Submission Deadline

**Submit by Saturday, 11:59 PM WAT**

Your work will be reviewed during the **Sunday review session** at [Time] UTC.

---

## Code of Conduct

We're building a community of excellence. Please follow these principles:

### Be Respectful
- Treat all community members with dignity
- Welcome diverse perspectives
- Assume good intent

### Be Supportive
- Help others learn and grow
- Share your knowledge generously
- Celebrate others' wins

### Give Constructive Feedback
- Focus on ideas, not people
- Provide specific, actionable suggestions
- Acknowledge what's working well

### Be Honest
- Document both successes and failures
- Share real metrics, not inflated numbers
- Admit when you don't know something

### No Plagiarism
- All work must be original
- Give credit when using others' ideas
- Don't copy code without attribution

### Respect Privacy
- Don't share personal information without consent
- Keep user data confidential
- Respect intellectual property

### Be Inclusive
- Welcome people from all backgrounds
- Use inclusive language
- Create space for everyone

**Violations may result in removal from the community.**

---

## Pull Request Process

### Before You Submit

1. **Check the guidelines**: Follow this guide
2. **Test your work**: Verify your live URL works
3. **Review your documentation**: Is it clear?
4. **Proofread**: Check for typos

### Submitting Your PR

1. **Create a descriptive title**:
   - ✅ "Week 3 Submission: Sarah Chen - Stripe Checkout Clone"
   - ❌ "Update files"

2. **Write a clear description**:
   ```markdown
   ## Week 3: Design-to-Code Mastery

   ### What I Built
   A Stripe Checkout clone with improved UX

   ### Live URL
   https://checkout-demo.vercel.app

   ### Key Metrics
   - Checkout completion rate: 82%
   - Average checkout time: 2.3 minutes
   - Error rate: 1.2%

   ### Challenges
   - Stripe test mode rate limiting (solved with retry logic)
   - Mobile responsiveness (solved with Tailwind breakpoints)

   ### Next Steps
   - Add discount code functionality
   - Implement abandoned cart recovery
   ```

3. **Include a checklist**:
   ```markdown
   - [x] I've provided a live URL
   - [x] I've linked to my GitHub repository
   - [x] I've documented key metrics
   - [x] I've included learnings and challenges
   - [x] I've proofread my documentation
   ```

### Review Process

1. **Community Review** (24-48 hours):
   - Community members may ask questions
   - Be responsive and open to feedback

2. **Mentor Review** (if applicable):
   - A mentor may review for quality
   - They may suggest improvements

3. **Approval & Merge**:
   - Once approved, your PR will be merged
   - Your work will be featured in the community

---

## Documentation Standards

### Writing Style

- **Be clear and concise**: Use short sentences
- **Use active voice**: "I built a dashboard" not "A dashboard was built"
- **Be specific**: "82% completion rate" not "good results"
- **Use examples**: Include code snippets and links

### Formatting

- **Use Markdown**: All documentation in `.md` format
- **Use headers**: Organize with H2 (`##`) and H3 (`###`)
- **Use lists**: Break up text with bullet points
- **Use code blocks**: Highlight code with triple backticks

```markdown
# Example Header

This is a paragraph with **bold** and *italic* text.

## Subheader

- Bullet point 1
- Bullet point 2

### Code Example

\`\`\`javascript
const greeting = "Hello, AI-Native PM!";
console.log(greeting);
\`\`\`

[Link to resource](https://example.com)
```

### File Naming

- Use lowercase with hyphens: `system-prompt.md`, `live-url.txt`
- Use descriptive names: `week-1-learnings.md` not `notes.md`
- Use consistent naming across all weeks

### Images & Media

- Store images in your week folder: `week-1/images/`
- Use descriptive alt text
- Keep file sizes reasonable
- Link to videos (Loom, YouTube) rather than uploading

---

## Sunday Review Sessions

### What Happens

Every Sunday at [Time] WAT, we gather to review submissions and celebrate wins.

**Format**:
- 3-5 participants demo their week's work (5 min each)
- Community provides feedback and asks questions
- Mentors share insights
- We celebrate wins and troubleshoot blockers

### How to Prepare

1. **Have your live URL ready**: Make sure it works
2. **Prepare a 5-minute demo**: What you built, key metrics, challenges
3. **Be ready for questions**: Think about potential feedback
4. **Bring your energy**: This is a celebration!

### Attendance

- **Optional but encouraged**: You'll get valuable feedback
- **Recording available**: Can't attend live? Watch the replay
- **Timezone-friendly**: We try to accommodate multiple timezones

### What to Expect

- **Positive feedback first**: We celebrate what worked
- **Constructive suggestions**: Ideas for improvement
- **Peer learning**: You'll learn from others' approaches
- **Networking**: Connect with fellow AI-Native PMs

---

## Sharing Knowledge

### Ways to Contribute Beyond Your Weekly Work

#### 1. Share Tool Guides
If you discover a useful tool or technique:
- Create a file: `resources/tool-guides/[tool-name].md`
- Include: What it is, how to use it, pros/cons, tutorial links

#### 2. Write Case Studies
Document interesting learnings:
- Create a file: `resources/case-studies/[topic].md`
- Include: Problem, solution, results, takeaways

#### 3. Answer Questions
Help other participants:
- Reply to discussions in GitHub Discussions
- Answer questions in Discord
- Share relevant resources

#### 4. Create Templates
Help others get started faster:
- Create a file: `resources/templates/[template-name].md`
- Include: Instructions, example, tips

#### 5. Fix Documentation
Improve existing resources:
- Find typos or unclear sections
- Submit a PR with improvements
- Add missing information

### Submitting Knowledge Contributions

1. Create a new branch: `git checkout -b feature/[contribution-name]`
2. Add your content to the appropriate folder
3. Commit and push: `git push origin feature/[contribution-name]`
4. Submit a PR with a clear description
5. Wait for review and approval

---

## Feedback & Reviews

### Giving Feedback

When reviewing others' work:

1. **Start with positives**: "I really liked how you..."
2. **Ask clarifying questions**: "How did you decide to...?"
3. **Provide specific suggestions**: "Consider adding... because..."
4. **Be encouraging**: "Great work! Here's how you could improve..."

### Receiving Feedback

When others review your work:

1. **Listen with an open mind**: Assume good intent
2. **Ask for clarification**: "Can you explain what you mean by...?"
3. **Thank them**: "Thanks for the feedback!"
4. **Iterate**: Use feedback to improve

### Feedback Channels

- **GitHub PR Comments**: For specific feedback
- **GitHub Discussions**: For general questions
- **Discord**: For real-time chat
- **Sunday Review**: For live feedback

---

## Common Questions

### Q: What if I don't finish a week?
**A**: That's okay. Document what you did and what you learned. Honesty is valued more than perfection.

### Q: Can I work with others?
**A**: Yes! Teams of 2-3 are encouraged. Each person must have their own portfolio repo, but you can collaborate.

### Q: What if my project fails?
**A**: Document what went wrong and why. That's worth more than a successful project with no learnings.

### Q: Can I go back and improve previous weeks?
**A**: Absolutely! You can update your submissions anytime. Just submit a new PR.

### Q: How do I get feedback on my work?
**A**: Submit a PR and ask for feedback. Mentors and community members will review and comment.

### Q: Can I use paid tools?
**A**: Yes, but the curriculum is designed to be 100% free. Document why you used paid tools if you do.

### Q: What if I'm stuck on a technical problem?
**A**: Ask in GitHub Discussions or Discord. The community is here to help.

### Q: Can I start at a different week?
**A**: No. Start with Week 1. The curriculum is sequential and builds on previous weeks.

### Q: What if I miss the Sunday review?
**A**: No problem. The recording will be available. You can watch it anytime.

### Q: How long do I have to complete the challenge?
**A**: There's no deadline. The challenge is forever open. You can work at your own pace.

### Q: What happens after Week 12?
**A**: The challenge continues. New weeks are added as new tools emerge. You can keep building or mentor others.

---

## Need Help?

- **Questions about the process?** Open an issue or discussion
- **Stuck on a technical problem?** Ask in Discord
- **Need mentorship?** Request a mentor in GitHub Issues
- **Have feedback on the guidelines?** Submit a PR with suggestions

---

## Important Links

- **Main README**: [README.md](./README.md)
- **Full Curriculum**: [CURRICULUM.md](./CURRICULUM.md)
- **Video Resources**: [resources/video-links.md](./resources/video-links.md)
- **Tool Guides**: [resources/tool-guides/](./resources/tool-guides/)
- **Community Showcase**: [COMMUNITY_SHOWCASE.md](./COMMUNITY_SHOWCASE.md)

### Community Channels

- **GitHub Discussions**: [Join the conversation](https://github.com/your-org/ai-native-pm-challenge/discussions)
- **Wahtsapp**: [Join our group](https://teams.microsoft.com/l/message/48:notes/1782768923385?context=%7B%22contextType%22%3A%22chat%22%2C%22oid%22%3A%228%3Aorgid%3Ae9a98708-7723-4ada-a949-0eff87980a04%22%7D)
- **Sunday Review**: [Teams Link](https://zoom.us/your-meeting-id)
- **Email**: [community@ai-native-pm.com](mailto:rahmotut@gmail.com)

---

## The Philosophy

> "Build the right thing fast — and prove it worked."

This challenge is for PMs who want to be **irreplaceable**. Who want to out-build engineers. Who want to own their future in the AI era.

**No options. No excuses. Just ship.**

---

## Thank You!

Thank you for being part of this community. Your contributions — whether code, documentation, feedback, or encouragement — help everyone grow.

Together, we're building the biggest AI-Native PM community in Africa.

---

**Last Updated**: June 2026  
**Maintained by**: AI-Native PM Community  
**Status**: Forever Open. Forever Evolving.

![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Focus](https://img.shields.io/badge/Focus-Africa-orange)
![Level](https://img.shields.io/badge/Level-Elite-blue)
