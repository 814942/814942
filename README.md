``` js
function presentation() {
  return {
    name: "Pablo",
    lastName: "Garay",
    age: 35,
    from: "Argentina",
    occupation: "Full Stack Developer" 
  }
}

function skills() {
  return {
    backEnd: [
      "Node.js",
      "Express",
      "Nestjs",
      "GraphQL",
      "Sequelize",
      "typeORM",
      "Postgres",
      "mySQL"
    ],
    frontEnd: [
      "HTML",
      "CSS",
      "React",
      "Nextjs",
      "Typescript",
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

// Copy and paste this line in ur console(F12) or right-click, select inspect and in the window that opens select console.
const english = hola("eng");
// Copia y pega estas lineas en tu consola(F12) o haz click con el boton secundario, selecciona inspeccionar y en la ventana que se abre consola.
const español = hola("esp");

STATS:
<img src="https://github.com/anuraghazra/github-readme-stats" width="120" height="120"/>
