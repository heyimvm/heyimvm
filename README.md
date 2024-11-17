const githubProfile = {
  username: "@heyimvm",
  interests: "😴 Sleeping all day",
  currentlyLearning: "🤖 To live like a human",
  contact: "📫 Don't reach me",
  funFact: "⭐ Starfish are cool!",
};

function generateReadme(profile) {
  return `
# Hi there! 👋

- 🔹 **Username:** ${profile.username}
- 🔹 **Interests:** ${profile.interests}
- 🔹 **Currently Learning:** ${profile.currentlyLearning}
- 🔹 **How to Reach Me:** ${profile.contact}
- 🔹 **Fun Fact:** ${profile.funFact}

> *"Keep calm and let the starfish shine!"*

---
✨ Made by ${profile.username} ✨
  `;
}
console.log(generateReadme(githubProfile));
