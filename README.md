
const profile = {
  username: "@heyimvm",
  interests: "Sleeping all day",
  currentlyLearning: "To live like a human",
  contact: "Don't reach me",
  funFacts: [
    "Starfish ⭐",
    "Dolphins sleep with one eye open 🐬",
    "Bananas are berries, but strawberries aren't 🍌",
    "The Eiffel Tower can grow taller in summer 🌞"
  ],
};

function displayProfile() {
  console.clear(); 
  console.log("=== My Profile ===");
  console.log(`👋 Hi, I’m ${profile.username}`);
  console.log(`👀 Interested in: ${profile.interests}`);
  console.log(`🌱 Currently learning: ${profile.currentlyLearning}`);
  console.log(`📫 How to reach me: ${profile.contact}`);
  console.log("⚡ Fun fact: " + profile.funFacts[0]);
  console.log("==================");
}

function showRandomFunFact() {
  const randomIndex = Math.floor(Math.random() * profile.funFacts.length);
  console.log("⚡ Random Fun Fact: " + profile.funFacts[randomIndex]);
}


function startInteraction() {
  let userInput;
  displayProfile();

  do {
    console.log("\nOptions:");
    console.log("1. Show another random fun fact");
    console.log("2. Display profile again");
    console.log("3. Exit");
    userInput = prompt("Enter your choice (1, 2, or 3):");

    switch (userInput) {
      case "1":
        showRandomFunFact();
        break;
      case "2":
        displayProfile();
        break;
      case "3":
        console.log("Goodbye! Hope you enjoyed the fun facts!");
        break;
      default:
        console.log("Invalid choice. Please enter 1, 2, or 3.");
    }
  } while (userInput !== "3");
}

startInteraction();
