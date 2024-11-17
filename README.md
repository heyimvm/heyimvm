
        "Dolphins sleep with one eye open 🐬",
        
        "Bananas are berries, but strawberries aren't 🍌",
        
        "The Eiffel Tower can grow taller in summer 🌞"
      ],
    };


    document.getElementById("interest").textContent = profile.interests;
    document.getElementById("learning").textContent = profile.currentlyLearning;
    document.getElementById("contact").textContent = profile.contact;
    document.getElementById("funFact").textContent = profile.funFacts[0];


    document.getElementById("changeFact").addEventListener("click", () => {
      const randomIndex = Math.floor(Math.random() * profile.funFacts.length);
      document.getElementById("funFact").textContent = profile.funFacts[randomIndex];
    });
