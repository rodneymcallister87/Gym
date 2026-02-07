<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gym Workout App</title>
<style>
body{margin:0;font-family:Arial,sans-serif;background:#f8f8f8;color:#222;}
header{padding:15px;background:#4a90e2;color:white;text-align:center;}
nav{display:flex;justify-content:space-around;background:#fff;padding:10px 0;box-shadow:0 2px 4px rgba(0,0,0,0.1);}
.navBtn{background:#4a90e2;color:white;border:none;padding:10px;border-radius:5px;}
main{padding:15px;}
.exercise-card{border:1px solid #ccc;padding:15px;margin:10px 0;background:#fff;border-radius:5px;}
input,button{padding:8px;margin:5px 0;width:100%;border-radius:5px;border:1px solid #ccc;}
iframe{margin-top:10px;border-radius:5px;}
</style>
</head>
<body>
<div id="app">
<header>
<h1>Gym Workout App</h1>
<button id="weightBtn">Log Bodyweight</button>
<span id="weightDisplay"></span>
</header>
<nav>
<button class="navBtn" data-screen="workouts">Workouts</button>
<button class="navBtn" data-screen="progress">Progress</button>
</nav>
<main id="mainContent"></main>
</div>

<script>
// --- Preloaded Data ---
let data = {
  "workouts":[
    {"name":"Upper Body","musicSpotify":"https://open.spotify.com/playlist/37i9dQZF1DX70RN3TfWWJh","musicYouTube":"https://www.youtube.com/playlist?list=PLtACth-r-xWBscDWqJHo8FnwMrFM7t3-3",
      "exercises":[
        {"id":"chest_press","name":"Seated Chest Press","recommendedWeight":100,"reps":"8–12","tutorial":"https://www.youtube.com/embed/X5HhM1IFkRk"},
        {"id":"lat_pulldown","name":"Lat Pulldown","recommendedWeight":130,"reps":"8–12","tutorial":"https://www.youtube.com/embed/CAwf7n6Luuc"},
        {"id":"shoulder_press","name":"Seated Dumbbell Shoulder Press","recommendedWeight":40,"reps":"8–12","tutorial":"https://www.youtube.com/embed/qEwKCR5JCog"},
        {"id":"one_arm_row","name":"One-Arm Dumbbell Row","recommendedWeight":50,"reps":"8–12","tutorial":"https://www.youtube.com/embed/pYcpY20QaE8"},
        {"id":"triceps_pushdown","name":"Triceps Pushdown","recommendedWeight":40,"reps":"10–12","tutorial":"https://www.youtube.com/embed/2-LAMcpzODU"},
        {"id":"bicep_curl","name":"Dumbbell Bicep Curl","recommendedWeight":25,"reps":"10–12","tutorial":"https://www.youtube.com/embed/ykJmrZ5v0Oo"}
      ]
    },
    {"name":"Lower Body","musicSpotify":"https://open.spotify.com/playlist/37i9dQZF1DWZzY0t7iVY0a","musicYouTube":"https://www.youtube.com/playlist?list=PL_UAXxDwtUkEexoG8TO-WXjJlfD8ScnwW",
      "exercises":[
        {"id":"goblet_squat","name":"Goblet Squat","recommendedWeight":40,"reps":"8–12","tutorial":"https://www.youtube.com/embed/UXJrBgI2RxA"},
        {"id":"romanian_deadlift","name":"Romanian Deadlift","recommendedWeight":65,"reps":"8–12","tutorial":"https://www.youtube.com/embed/2SHsk9AzdjA"},
        {"id":"leg_press","name":"Leg Press","recommendedWeight":180,"reps":"10–12","tutorial":"https://www.youtube.com/embed/IZxyjW7MPJQ"},
        {"id":"step_up","name":"Step-Ups","recommendedWeight":25,"reps":"10 each leg","tutorial":"https://www.youtube.com/embed/dQqApCGd5Ss"},
        {"id":"calf_raise","name":"Standing Calf Raise","recommendedWeight":90,"reps":"12–15","tutorial":"https://www.youtube.com/embed/Yl5r8PeHf0g"}
      ]
    },
    {"name":"Core & Cardio","musicSpotify":"https://open.spotify.com/playlist/37i9dQZF1DWZkWfQ2m0W1u","musicYouTube":"https://www.youtube.com/playlist?list=PLqrqH3WSfDVmqz4c8i4qw_8SaHrTa4kka",
      "exercises":[
        {"id":"plank","name":"Plank (modified)","recommendedWeight":0,"reps":"20–40 sec","tutorial":"https://www.youtube.com/embed/pSHjTRCQxIw"},
        {"id":"dead_bug","name":"Dead Bug","recommendedWeight":0,"reps":"10 each side","tutorial":"https://www.youtube.com/embed/2HRmq8g46YQ"},
        {"id":"cable_crunch","name":"Standing Cable Crunch","recommendedWeight":50,"reps":"12–15","tutorial":"https://www.youtube.com/embed/Y6_H8Fz10N0"}
      ]
    }
  ],
  "bodyweights":[]
};

// --- Functions ---
function showWorkouts(){
  const main=document.getElementById("mainContent"); main.innerHTML="";
  data.workouts.forEach((w,i)=>{
    const btn=document.createElement("button"); btn.textContent=w.name;
    btn.onclick=()=>openWorkout(i);
    main.appendChild(btn);
  });
}

function openWorkout(index){
  const main=document.getElementById("mainContent"); const workout=data.workouts[index];
  main.innerHTML=`<h2>${workout.name}</h2>
    <button onclick="openMusic('${workout.musicSpotify}','${workout.musicYouTube}')">Start Music</button>`;
  workout.exercises.forEach(ex=>{
    const card=document.createElement("div"); card.className="exercise-card";
    card.innerHTML=`<h3>${ex.name}</h3>
      <iframe width="100%" height="200" src="${ex.tutorial}" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
      <p>Recommended: ${ex.recommendedWeight} lbs — Reps: ${ex.reps}</p>
      <input type="number" id="${ex.id}_w" placeholder="Weight used (lbs)">
      <input type="number" id="${ex.id}_r" placeholder="Reps">
      <button onclick="logSet('${ex.id}')">Log Set</button>`;
    main.appendChild(card);
  });
}

function openMusic(spotify,yt){
  if(spotify) window.open(spotify,"_blank");
  else if(yt) window.open(yt,"_blank");
  else alert("No playlist links available.");
}

function logSet(id){
  const w=parseInt(document.getElementById(`${id}_w`).value);
  const r=parseInt(document.getElementById(`${id}_r`).value);
  if(!w||!r) return alert("Enter weight and reps");
  const ex=data.workouts.flatMap(wk=>wk.exercises).find(e=>e.id===id);
  if(r>=parseInt(ex.reps.split('–')[1])) ex.recommendedWeight=Math.round(ex.recommendedWeight*1.05);
  else if(r<parseInt(ex.reps.split('–')[0])) ex.recommendedWeight=Math.max(5,ex.recommendedWeight-5);
  alert(`Logged ${w} lbs x ${r} reps\nNext recommended: ${ex.recommendedWeight} lbs`);
}

document.getElementById("weightBtn").onclick=()=>{
  const w=prompt("Enter your current bodyweight (lbs) for this week:");
  if(w){data.bodyweights.push({date:new Date().toISOString(),weight:w});
    document.getElementById("weightDisplay").textContent=`Last: ${w} lbs`;
  }
};

document.querySelectorAll(".navBtn").forEach(btn=>{
  btn.onclick=()=>{btn.dataset.screen==="workouts"?showWorkouts():showProgress();}
});

function showProgress(){
  const main=document.getElementById("mainContent"); main.innerHTML="<h2>Weekly Bodyweight Progress</h2>";
  if(data.bodyweights.length===0){main.innerHTML+="<p>No data logged yet.</p>"; return;}
  let list="<ul>"; data.bodyweights.forEach(entry=>list+=`<li>${new Date(entry.date).toLocaleDateString()}: ${entry.weight} lbs</li>`); list+="</ul>";
  main.innerHTML+=list;
}

// Initial load
showWorkouts();
</script>
</body>
</html>
