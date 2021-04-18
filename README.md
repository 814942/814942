``` js
function presentation() {
  return {
    name: "Pablo",
    lastName: "Garay",
    age: 32,
    from: "Argentina",
    occupation: "Full Stack Developer" 
  }
}

function skills() {
  return {
    backEnd: [
      "Node.js",
      "Express",
      "GraphQL",
      "Sequelize",
      "Postgres"
    ],
    frontEnd: [
      "HTML",
      "CSS",
      "React",
      "Redux"
    ]
  }
}

function hobbies() {
  return "🎮 gammer, 🎥 cinefilo, 🏍️ motorcyclist";
}

function hola(language) {
  let me = presentation();
  let mySkills = skills();
  let myHobbies = hobbies();
  
  language === "eng" 
  ? console.log(`Hello there 😀 my name is ${me.name} ${me.lastName}, i´m ${me.age} years old, i´m from ${me.from} and i´m ${me.occupation}. My hobbies are: ${myHobbies}. Some of my skills are: `)
  : console.log(`Hola 😀 mi nombre es ${me.name} ${me.lastName}, tengo ${me.age} años, soy de ${me.from} y soy ${me.occupation}. Mis hobbies son: ${myHobbies}. Algunas de mis habilidades son: `);
  
  console.table(mySkills)
}

const english = hola("eng");
const español = hola("esp");
