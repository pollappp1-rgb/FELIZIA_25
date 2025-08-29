<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>Felizia Inter Campus Fest | Muhyissunna Students' Association</title>
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <style>
    :root {
      --bg: #0b1117;
      --panel: #111a23;
      --muted: #7b8a9b;
      --text: #e6eef7;
      --accent: #2f89ff;
      --accent-2: #22c55e;
      --warn: #f59e0b;
      --danger: #ef4444;
      --border: #1e2a35;
      --chip: #0f1720;
    }
    * { box-sizing: border-box; }
    body {
      margin: 0; background: var(--bg); color: var(--text);
      font: 14px/1.5 Inter, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji","Segoe UI Emoji";
    }
    a { color: var(--accent); text-decoration: none; }
    input, select, button, textarea {
      background: #0e1620; border: 1px solid var(--border); color: var(--text); border-radius: 8px; padding: 10px;
      outline: none; width: 100%;
    }
    button { cursor: pointer; background: var(--accent); border: none; color: white; font-weight: 600; }
    button.secondary { background: #0e1620; border: 1px solid var(--border); }
    button.success { background: var(--accent-2); }
    button.warn { background: var(--warn); color: #0b1117; }
    button.danger { background: var(--danger); }
    button.ghost { background: transparent; border: 1px solid var(--border); }
    button:disabled { opacity: .6; cursor: not-allowed; }
    label { display: block; margin: 10px 0 6px; color: var(--muted); }
    .container { max-width: 1280px; margin: 0 auto; padding: 20px; }
    .card { background: var(--panel); border: 1px solid var(--border); border-radius: 12px; padding: 16px; }
    .row { display: grid; grid-template-columns: 1fr; gap: 16px; }
    @media(min-width: 900px){ .row-2{ grid-template-columns: 1fr 1fr; } .row-3 { grid-template-columns: 1fr 1fr 1fr; } }
    .flex { display: flex; gap: 10px; align-items: center; }
    .flex-wrap { flex-wrap: wrap; }
    .space { flex: 1; }
    .muted { color: var(--muted); }
    .badge { display: inline-block; padding: 4px 8px; background: var(--chip); border: 1px solid var(--border); border-radius: 999px; font-size: 12px; }
    .pill { padding: 6px 10px; border-radius: 999px; }
    .mono { font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", monospace; }
    .hidden { display: none !important; }
    .tabs { display: flex; gap: 6px; border-bottom: 1px solid var(--border); padding-bottom: 6px; margin-bottom: 16px; flex-wrap: wrap; }
    .tab { padding: 8px 14px; border-radius: 10px; cursor: pointer; border: 1px solid var(--border); background: #0c141c; }
    .tab.active { background: #0e1620; color: white; }
    .table { width: 100%; border-collapse: collapse; }
    .table th, .table td { border-bottom: 1px solid var(--border); padding: 10px; vertical-align: top; }
    .table th { text-align: left; color: var(--muted); font-weight: 600; }
    .grid { display: grid; gap: 10px; }
    .grid-2 { grid-template-columns: 1fr 1fr; }
    .grid-3 { grid-template-columns: 1fr 1fr 1fr; }
    .grid-4 { grid-template-columns: repeat(4, 1fr); }
    .head { display: flex; gap: 12px; align-items: center; margin-bottom: 12px; }
    .h1 { font-size: 22px; font-weight: 700; }
    .h2 { font-size: 18px; font-weight: 700; }
    .h3 { font-size: 16px; font-weight: 700; }
    .sub { font-size: 12px; color: var(--muted); }
    .hr { border-bottom: 1px solid var(--border); margin: 16px 0; }
    .kpi { padding: 12px; border-radius: 10px; background: #0d1520; border: 1px solid var(--border); }
    .chip { background: #0f1720; border: 1px solid var(--border); border-radius: 6px; padding: 4px 6px; font-size: 12px; }
    .center { text-align: center; }
    .right { text-align: right; }
    .danger-text { color: var(--danger); }
    .success-text { color: var(--accent-2); }
    .warn-text { color: var(--warn); }
    .link { color: var(--accent); cursor: pointer; }
    .sticky { position: sticky; top: 0; z-index: 8; background: var(--bg); padding-top: 10px; }
    .mini { font-size: 12px; }
    .list { list-style: none; padding: 0; margin: 0; }
    .list li { border-bottom: 1px solid var(--border); padding: 8px 0; }
    .toast { position: fixed; bottom: 14px; right: 14px; background: #0e1620; border: 1px solid var(--border); border-radius: 10px; padding: 10px 12px; z-index: 100; }
    .ok { color: var(--accent-2); }
    .warnc { color: var(--warn); }
    .err { color: var(--danger); }
    .note { padding: 10px; border: 1px dashed var(--border); border-radius: 10px; color: var(--muted); background: #0c141c; }
    .print-area { background: white; color: black; padding: 16px; }
    .code { background: #0e1620; border: 1px solid var(--border); border-radius: 10px; padding: 8px; }
  </style>
</head>
<body>
  <div class="container">
    <div id="appRoot">
      <!-- Login -->
      <div id="viewLogin" class="card">
        <div class="head">
          <div class="h1">Felizia Inter Campus Fest</div>
          <span class="badge">Muhyissunna Students' Association</span>
        </div>
        <div class="row row-2">
          <div>
            <div class="h2">Sign in</div>
            <div class="sub">Choose your role and enter credentials</div>
            <div class="hr"></div>
            <label>Role</label>
            <select id="loginRole">
              <option value="team">Team Portal (Participation Crew)</option>
              <option value="event">Event Crew (Admin)</option>
            </select>
            <label>ID (email or team ID)</label>
            <input id="loginEmail" placeholder="e.g., qairuwan@felizia or admin@felizia" />
            <label>Password</label>
            <input id="loginPass" type="password" placeholder="Your password" />
            <div class="flex" style="margin-top:10px;">
              <button id="btnLogin">Sign in</button>
              <button id="btnDemo" class="secondary">Use Local Demo Mode</button>
              <span class="space"></span>
              <span class="muted mini">Admin can manage accounts in Event Crew → Teams</span>
            </div>
            <div id="loginMsg" class="mini muted" style="margin-top:8px;"></div>
            <div class="note" style="margin-top:12px;">
              To enable multi-device online mode, configure Firebase in the code (see bottom of this file for steps).
            </div>
          </div>
          <div>
            <div class="card">
              <div class="h3">Quick facts</div>
              <ul class="list">
                <li>Teams: Qairuwan, Rabath, Fustat, Qazween</li>
                <li>Categories: Lower, Primary, Minor, High, Major, Popular</li>
                <li>Event Crew controls lock/unlock, points, bonuses, penalties</li>
                <li>Team privacy: one team can’t see others’ entries</li>
                <li>Judge Panel: post results anytime, editable</li>
                <li>Poster generator for winners</li>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <!-- Team Portal -->
      <div id="viewTeam" class="hidden">
        <div class="sticky">
          <div class="flex">
            <div class="h2">Team Portal — <span id="teamNameHdr"></span></div>
            <span id="teamLockBadge" class="badge"></span>
            <span class="space"></span>
            <input id="teamSearch" placeholder="Search student or competition..." style="max-width:360px;" />
            <button id="btnLogoutTeam" class="ghost">Log out</button>
          </div>
          <div class="tabs">
            <div class="tab active" data-team-tab="students">Students</div>
            <div class="tab" data-team-tab="register">Register Participation</div>
            <div class="tab" data-team-tab="mycomps">My Competitions</div>
            <div class="tab" data-team-tab="list">Participation List</div>
          </div>
        </div>

        <div id="teamTab-students" class="card">
          <div class="row row-2">
            <div>
              <div class="h3">Add Student</div>
              <div class="grid">
                <div>
                  <label>Chest No</label>
                  <input id="tAddChest" />
                </div>
                <div>
                  <label>Name</label>
                  <input id="tAddName" />
                </div>
                <div>
                  <label>Category</label>
                  <select id="tAddCat"></select>
                </div>
              </div>
              <div class="flex" style="margin-top:10px;">
                <button id="btnAddStudent">Add Student</button>
                <span id="tAddMsg" class="mini muted"></span>
              </div>
              <div class="note" style="margin-top:12px;">
                Only your team members are visible here. Chest numbers must be unique within your team.
              </div>
            </div>
            <div>
              <div class="h3">Students</div>
              <table class="table" id="tblTeamStudents">
                <thead><tr>
                  <th>Chest</th><th>Name</th><th>Category</th><th>Competitions</th><th></th>
                </tr></thead>
                <tbody></tbody>
              </table>
            </div>
          </div>
        </div>

        <div id="teamTab-register" class="card hidden">
          <div class="row row-2">
            <div>
              <div class="h3">Select Student</div>
              <select id="selRegStudent"></select>
              <div id="regStuInfo" class="mini muted" style="margin-top:8px;"></div>
              <div class="hr"></div>
              <div class="h3">Available Competitions</div>
              <div id="regCompList"></div>
            </div>
            <div>
              <div id="groupBox" class="hidden">
                <div class="h3">Group Entry</div>
                <label>Group Name (optional)</label>
                <input id="groupName" placeholder="e.g., Qairuwan Juniors" />
                <label>Add Members (same team; same category unless Popular)</label>
                <div id="groupMembers"></div>
              </div>
              <div id="capInfo" class="note">
                Capacity and rules are enforced automatically by the system.
              </div>
            </div>
          </div>
        </div>

        <div id="teamTab-mycomps" class="card hidden">
          <div class="h3">Team’s Competition Entries</div>
          <div id="teamCompEntries"></div>
        </div>

        <div id="teamTab-list" class="card hidden">
          <div class="flex">
            <div>
              <div class="h3">Comprehensive Participation List</div>
              <div class="sub">Name, Chest No, Category, Competitions</div>
            </div>
            <span class="space"></span>
            <button id="btnPrintTeamList" class="ghost">Print</button>
          </div>
          <div id="teamParticipationList"></div>
        </div>
      </div>

      <!-- Event Crew Portal -->
      <div id="viewEvent" class="hidden">
        <div class="sticky">
          <div class="flex">
            <div class="h2">Event Crew Portal</div>
            <span class="space"></span>
            <input id="eventSearch" placeholder="Search student or competition..." style="max-width:400px;" />
            <button id="btnLogoutEvent" class="ghost">Log out</button>
          </div>
          <div class="tabs">
            <div class="tab active" data-event-tab="dashboard">Dashboard</div>
            <div class="tab" data-event-tab="teams">Teams</div>
            <div class="tab" data-event-tab="competitions">Competitions</div>
            <div class="tab" data-event-tab="attendance">Attendance</div>
            <div class="tab" data-event-tab="judge">Judge Panel</div>
            <div class="tab" data-event-tab="scoreboard">Scoreboards</div>
            <div class="tab" data-event-tab="poster">Poster Generator</div>
          </div>
        </div>

        <div id="eventTab-dashboard" class="card">
          <div class="row row-3">
            <div class="kpi"><div class="muted">Total Students</div><div id="kpiStudents" class="h1">0</div></div>
            <div class="kpi"><div class="muted">Competitions</div><div id="kpiComps" class="h1">0</div></div>
            <div class="kpi"><div class="muted">Total Participations</div><div id="kpiParts" class="h1">0</div></div>
          </div>
          <div class="hr"></div>
          <div class="row row-2">
            <div>
              <div class="h3">Winners Feed (Latest)</div>
              <ul id="winnersFeed" class="list"></ul>
            </div>
            <div>
              <div class="h3">Top Teams (Overall)</div>
              <table class="table" id="tblTopTeams"><thead>
                <tr><th>Team</th><th class="right">Points</th></tr>
              </thead><tbody></tbody></table>
            </div>
          </div>
        </div>

        <div id="eventTab-teams" class="card hidden">
          <div class="flex">
            <div class="h3">Teams</div>
            <span class="space"></span>
            <button id="btnSeedTeams" class="secondary">Initialize Default Teams</button>
          </div>
          <table class="table" id="tblTeams">
            <thead><tr>
              <th>Team</th><th>Status</th><th>Bonus</th><th>Penalty</th><th class="right">Actions</th>
            </tr></thead>
            <tbody></tbody>
          </table>
          <div class="hr"></div>
          <div class="h3">Accounts (create for login)</div>
          <div class="row row-3">
            <div class="card">
              <div class="h3">Add Team Account</div>
              <label>Team</label>
              <select id="accTeam"></select>
              <label>Email (ID)</label>
              <input id="accEmail" placeholder="e.g., qairuwan@felizia" />
              <label>Password</label>
              <input id="accPass" type="password" />
              <button id="btnCreateTeamAccount">Create Team Account</button>
              <div id="accMsg" class="mini muted" style="margin-top:8px;"></div>
            </div>
            <div class="card">
              <div class="h3">Add Event Crew Account</div>
              <label>Email (ID)</label>
              <input id="accEventEmail" placeholder="e.g., admin@felizia" />
              <label>Password</label>
              <input id="accEventPass" type="password" />
              <button id="btnCreateEventAccount">Create Event Crew Account</button>
              <div id="accEventMsg" class="mini muted" style="margin-top:8px;"></div>
            </div>
            <div class="card note">
              Accounts are stored under “profiles” with role and team assignment. Security rules restrict access appropriately.
            </div>
          </div>
        </div>

        <div id="eventTab-competitions" class="card hidden">
          <div class="row row-2">
            <div>
              <div class="h3">Create Competition</div>
              <label>Name</label>
              <input id="cName" placeholder="e.g., Malayalam Elocution" />
              <label>Category</label>
              <select id="cCat"></select>
              <label>Type</label>
              <select id="cType">
                <option value="individual">Individual</option>
                <option value="group">Group</option>
              </select>
              <label>Max per Team</label>
              <input id="cMaxTeam" type="number" min="1" value="3" />
              <button id="btnAddComp">Add Competition</button>
              <div class="mini muted" id="cMsg" style="margin-top:8px;"></div>
            </div>
            <div>
              <div class="h3">Competitions</div>
              <table class="table" id="tblComps">
                <thead><tr>
                  <th>Name</th><th>Category</th><th>Type</th><th>Max/Team</th><th class="right">Actions</th>
                </tr></thead>
                <tbody></tbody>
              </table>
            </div>
          </div>
        </div>

        <div id="eventTab-attendance" class="card hidden">
          <div class="h3">Attendance & Code Letters</div>
          <label>Select Competition</label>
          <select id="attSelComp"></select>
          <div id="attList"></div>
        </div>

        <div id="eventTab-judge" class="card hidden">
          <div class="h3">Judge Panel — Results Entry</div>
          <label>Select Competition</label>
          <select id="judgeSelComp"></select>
          <div id="judgeList"></div>
          <div class="hr"></div>
          <div class="h3">Winners</div>
          <div id="winnersEditor"></div>
          <div class="flex" style="margin-top:8px;">
            <button id="btnSaveResults" class="success">Save/Update Results</button>
            <div id="judgeMsg" class="mini muted"></div>
          </div>
        </div>

        <div id="eventTab-scoreboard" class="card hidden">
          <div class="row row-2">
            <div>
              <div class="h3">Overall Scoreboard</div>
              <table class="table" id="tblScoreOverall">
                <thead><tr><th>Team</th><th class="right">Points</th></tr></thead>
                <tbody></tbody>
              </table>
            </div>
            <div>
              <div class="h3">Category Champions</div>
              <div id="catChampions"></div>
            </div>
          </div>
          <div class="hr"></div>
          <div class="h3">Winners by Category</div>
          <div id="winnersByCat"></div>
        </div>

        <div id="eventTab-poster" class="card hidden">
          <div class="row row-2">
            <div>
              <div class="h3">Poster Generator</div>
              <div class="note">Load your template image (PNG/JPG), then add text. You can also autofill from a selected winner.</div>
              <label>Template Image</label>
              <input id="postImg" type="file" accept="image/*" />
              <label>Text Lines</label>
              <div class="grid">
                <input id="postLine1" placeholder="Name (e.g., Minhaj)" />
                <input id="postLine2" placeholder="Category (e.g., Lower Zone)" />
                <input id="postLine3" placeholder="Event & Place (e.g., Malayalam Elocution — 1st)" />
              </div>
              <div class="grid grid-3" style="margin-top:8px;">
                <div><label>Font</label><input id="postFont" value="bold 48px Inter" /></div>
                <div><label>Text Color</label><input id="postColor" value="#ffffff" /></div>
                <div><label>Shadow</label><input id="postShadow" value="rgba(0,0,0,0.6)" /></div>
              </div>
              <div class="grid grid-3" style="margin-top:8px;">
                <div><label>Line1 Y</label><input id="y1" type="number" value="200" /></div>
                <div><label>Line2 Y</label><input id="y2" type="number" value="260" /></div>
                <div><label>Line3 Y</label><input id="y3" type="number" value="320" /></div>
              </div>
              <div class="flex" style="margin-top:8px;">
                <button id="btnRenderPoster">Render</button>
                <button id="btnDownloadPoster" class="secondary">Download PNG</button>
              </div>
              <div class="hr"></div>
              <div class="h3">Autofill from Winner</div>
              <label>Choose Competition</label>
              <select id="postComp"></select>
              <label>Winner Place</label>
              <select id="postPlace">
                <option value="1">1st</option>
                <option value="2">2nd</option>
                <option value="3">3rd</option>
              </select>
              <button id="btnAutofillPoster" class="ghost" style="margin-top:8px;">Autofill Text</button>
            </div>
            <div>
              <canvas id="posterCanvas" width="1200" height="628" style="width:100%;background:#000;border-radius:10px;border:1px solid var(--border);"></canvas>
            </div>
          </div>
        </div>
      </div>

      <!-- Toast -->
      <div id="toast" class="toast hidden"><span id="toastText"></span></div>

      <!-- Print -->
      <div id="printArea" class="hidden"></div>
    </div>
  </div>

  <!-- Firebase (optional for online mode) -->
  <script type="module">
    // ========= CONFIG =========
    // To use multi-device online mode:
    // 1) Create a Firebase project (Authentication + Firestore)
    // 2) Fill firebaseConfig below
    // 3) Deploy rules from "firestore.rules" (see end of this file)
    // If you do not configure Firebase, app runs in local demo mode.
    const firebaseConfig = {
      apiKey: "CHANGE_ME",
      authDomain: "CHANGE_ME.firebaseapp.com",
      projectId: "CHANGE_ME",
      storageBucket: "CHANGE_ME.appspot.com",
      messagingSenderId: "CHANGE_ME",
      appId: "CHANGE_ME"
    };

    // ========= GLOBALS =========
    const CATEGORIES = ["Lower Zone","Primary Zone","Minor Zone","High Zone","Major Zone","Popular Zone"];
    const TEAMS = ["Qairuwan","Rabath","Fustat","Qazween"];
    const State = {
      mode: "local", // "local" or "cloud"
      uid: null,
      role: null, // "team" or "event"
      teamId: null, // for team role
      // caches
      teams: {},      // by id
      students: {},   // by id
      competitions: {}, // by id
      participations: {}, // by id
      results: {},    // by competitionId
      profiles: {}, // uid -> {role, teamId}
      // UI
      listening: false,
    };

    // ========= UTIL =========
    const $ = (sel, root=document) => root.querySelector(sel);
    const $$ = (sel, root=document) => Array.from(root.querySelectorAll(sel));
    const safe = (s) => String(s||"");
    const id = () => Math.random().toString(36).slice(2) + Date.now().toString(36);
    const toast = (msg, cls="") => {
      const t = $("#toast"); $("#toastText").textContent = msg; t.classList.remove("hidden");
      t.classList.remove("ok","warnc","err"); if (cls) t.classList.add(cls);
      setTimeout(()=>t.classList.add("hidden"), 1800);
    };
    const fmtTeam = (t)=>t;
    const fmtCat = (c)=>c;

    function groupBy(arr, keyFn){
      const m = new Map();
      for(const x of arr){ const k = keyFn(x); if(!m.has(k)) m.set(k,[]); m.get(k).push(x); }
      return m;
    }

    // ========= BACKENDS =========
    // Local store (demo/offline)
    const LocalStore = {
      init(){ /* load from localStorage */ 
        const load = k => { try { return JSON.parse(localStorage.getItem(k)||"{}"); } catch{ return {}; } };
        State.teams = load("teams") || {};
        State.students = load("students") || {};
        State.competitions = load("competitions") || {};
        State.participations = load("participations") || {};
        State.results = load("results") || {};
        State.profiles = load("profiles") || {};
        // seed teams if empty
        if(Object.keys(State.teams).length===0){
          for(const t of TEAMS){ State.teams[t] = { id: t, name: t, locked: false, bonus: 0, penalty: 0 }; }
          this._save("teams", State.teams);
        }
        // minimal default admin account and team accounts for local demo
        if(Object.keys(State.profiles).length===0){
          // event admin
          State.profiles["admin@felizia"] = { uid:"admin@felizia", role:"event", teamId:null, pass:"admin123" };
          // teams
          for(const t of TEAMS){
            const email = t.toLowerCase()+"@felizia";
            State.profiles[email] = { uid:email, role:"team", teamId:t, pass:"team123" };
          }
          this._save("profiles", State.profiles);
        }
      },
      _save(key, obj){ localStorage.setItem(key, JSON.stringify(obj)); },
      async signIn(email, pass){
        const u = State.profiles[email];
        if(!u || u.pass !== pass) throw new Error("Invalid credentials");
        State.uid = u.uid; State.role = u.role; State.teamId = u.teamId || null;
        return u;
      },
      async signOut(){ State.uid=null; State.role=null; State.teamId=null; },
      async createAccount({email, pass, role, teamId}){
        if(State.profiles[email]) throw new Error("Account exists");
        State.profiles[email] = { uid:email, role, teamId: role==="team"? teamId : null, pass };
        this._save("profiles", State.profiles);
        return true;
      },
      // Teams
      async seedTeams(){
        for(const t of TEAMS){ State.teams[t] = { id:t, name:t, locked:false, bonus:0, penalty:0 }; }
        this._save("teams", State.teams);
      },
      async updateTeam(id, patch){
        const t = State.teams[id]; if(!t) throw new Error("Team not found");
        Object.assign(t, patch); this._save("teams", State.teams);
      },
      // Students
      async addStudent(stu){
        const sid = stu.id || id(); stu.id = sid;
        // uniqueness chest per team
        for(const s of Object.values(State.students)){
          if(s.teamId===stu.teamId && String(s.chestNo).trim()===String(stu.chestNo).trim()){
            throw new Error("Chest number already exists in your team");
          }
        }
        State.students[sid]=stu; this._save("students", State.students);
        return sid;
      },
      async removeStudent(sid){
        delete State.students[sid]; this._save("students", State.students);
        // remove from groups if needed
        for(const [pid,p] of Object.entries(State.participations)){
          if(p.studentIds && p.studentIds.includes(sid)){
            p.studentIds = p.studentIds.filter(x=>x!==sid);
            this._save("participations", State.participations);
          }
        }
      },
      // Competitions
      async addCompetition(c){
        c.id = id();
        State.competitions[c.id]=c; this._save("competitions", State.competitions); return c.id;
      },
      async removeCompetition(cid){
        delete State.competitions[cid]; this._save("competitions", State.competitions);
        // cleanup participations/results
        for(const [pid,p] of Object.entries(State.participations)){ if(p.competitionId===cid) delete State.participations[pid]; }
        this._save("participations", State.participations);
        delete State.results[cid]; this._save("results", State.results);
      },
      // Participation
      async addParticipation(p){
        // enforce max per team
        const comp = State.competitions[p.competitionId];
        const teamCount = Object.values(State.participations).filter(x=>x.competitionId===p.competitionId && x.teamId===p.teamId).length;
        if(teamCount >= Number(comp.maxPerTeam||0)) throw new Error("Team capacity reached for this competition");
        p.id = id(); p.attendance = false; p.codeLetter = p.codeLetter || "";
        State.participations[p.id]=p; this._save("participations", State.participations);
        return p.id;
      },
      async updateParticipation(pid, patch){
        const p = State.participations[pid]; if(!p) throw new Error("Not found");
        Object.assign(p, patch); this._save("participations", State.participations);
      },
      async removeParticipation(pid){
        delete State.participations[pid]; this._save("participations", State.participations);
      },
      // Results
      async saveResults(compId, winnersArr){
        State.results[compId] = { competitionId: compId, winners: winnersArr };
        this._save("results", State.results);
      },
      // Readers
      subscribeAll(cb){
        // In local mode, we just call cb immediately; no realtime
        cb();
        return ()=>{};
      }
    };

    // Firestore store (online/cloud)
    let app, auth, db;
    let onUnsub = null;
    const CloudStore = {
      async init(){
        // rudimentary check
        if(!firebaseConfig || firebaseConfig.apiKey==="CHANGE_ME") { State.mode = "local"; return LocalStore.init(); }
        const { initializeApp } = await import("https://www.gstatic.com/firebasejs/10.12.2/firebase-app.js");
        const { getAuth, signInWithEmailAndPassword, signOut, createUserWithEmailAndPassword, onAuthStateChanged } = await import("https://www.gstatic.com/firebasejs/10.12.2/firebase-auth.js");
        const { getFirestore, collection, doc, getDoc, setDoc, addDoc, updateDoc, deleteDoc, onSnapshot, query } = await import("https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore.js");
        app = initializeApp(firebaseConfig);
        auth = getAuth(app);
        db = getFirestore(app);
        State.mode = "cloud";
        // realtime listeners
        this._mountRealtime();
        // expose auth functions
        this._auth = { signInWithEmailAndPassword, signOut, createUserWithEmailAndPassword, onAuthStateChanged };
        this._fs = { collection, doc, getDoc, setDoc, addDoc, updateDoc, deleteDoc, onSnapshot, query };
      },
      async signIn(email, pass){
        const u = await this._auth.signInWithEmailAndPassword(auth, email, pass);
        State.uid = u.user.uid;
        // load profile
        const ref = this._fs.doc(db, "profiles", State.uid);
        const snap = await this._fs.getDoc(ref);
        if(!snap.exists()) throw new Error("Profile not found for this account");
        const prof = snap.data();
        State.role = prof.role; State.teamId = prof.role==="team"? prof.teamId : null;
        return prof;
      },
      async signOut(){ await this._auth.signOut(auth); State.uid=null; State.role=null; State.teamId=null; },
      async createAccount({email, pass, role, teamId}){
        if(State.role!=="event") throw new Error("Only Event Crew can create accounts");
        const u = await this._auth.createUserWithEmailAndPassword(auth, email, pass);
        const profRef = this._fs.doc(db,"profiles",u.user.uid);
        await this._fs.setDoc(profRef, { role, teamId: role==="team"? teamId : null, email });
        return true;
      },
      async seedTeams(){
        for(const t of TEAMS){
          const ref = this._fs.doc(db, "teams", t);
          await this._fs.setDoc(ref, { id:t, name:t, locked:false, bonus:0, penalty:0 }, { merge:true });
        }
      },
      async updateTeam(id, patch){
        const ref = this._fs.doc(db,"teams",id); await this._fs.updateDoc(ref, patch);
      },
      async addStudent(stu){
        // chest uniqueness must be enforced client-side + optionally by querying; Firestore does not allow unique constraints
        // Simple check in cache:
        for(const s of Object.values(State.students)){ if(s.teamId===stu.teamId && String(s.chestNo).trim()===String(stu.chestNo).trim()) throw new Error("Chest number already exists in your team"); }
        const { addDoc, collection } = this._fs;
        const ref = await addDoc(collection(db,"students"), stu);
        return ref.id;
      },
      async removeStudent(sid){
        const { doc, deleteDoc } = this._fs;
        await deleteDoc(doc(db,"students",sid));
      },
      async addCompetition(c){
        const { addDoc, collection } = this._fs;
        const ref = await addDoc(collection(db,"competitions"), c); return ref.id;
      },
      async removeCompetition(cid){
        const { doc, deleteDoc } = this._fs;
        await deleteDoc(doc(db,"competitions",cid));
        // participations and results cleanup: recommend Cloud Function; here we rely on UI preventing orphan reads.
      },
      async addParticipation(p){
        // enforce max per team (client-side from cache)
        const comp = State.competitions[p.competitionId];
        const teamCount = Object.values(State.participations).filter(x=>x.competitionId===p.competitionId && x.teamId===p.teamId).length;
        if(teamCount >= Number(comp.maxPerTeam||0)) throw new Error("Team capacity reached for this competition");
        const { addDoc, collection } = this._fs;
        const ref = await addDoc(collection(db,"participations"), p); return ref.id;
      },
      async updateParticipation(pid, patch){
        const { doc, updateDoc } = this._fs; await updateDoc(doc(db,"participations",pid), patch);
      },
      async removeParticipation(pid){
        const { doc, deleteDoc } = this._fs; await deleteDoc(doc(db,"participations",pid));
      },
      async saveResults(compId, winnersArr){
        const { doc, setDoc } = this._fs;
        await setDoc(doc(db,"results",compId), { competitionId: compId, winners: winnersArr }, { merge:true });
      },
      subscribeAll(cb){
        const { collection, onSnapshot } = this._fs;
        const unsubs = [];
        unsubs.push(onSnapshot(collection(db,"teams"), snap=>{
          State.teams = {}; snap.forEach(d=>State.teams[d.id]=d.data()); cb();
        }));
        unsubs.push(onSnapshot(collection(db,"students"), snap=>{
          State.students = {}; snap.forEach(d=>State.students[d.id]={...d.data(), id:d.id}); cb();
        }));
        unsubs.push(onSnapshot(collection(db,"competitions"), snap=>{
          State.competitions = {}; snap.forEach(d=>State.competitions[d.id]={...d.data(), id:d.id}); cb();
        }));
        unsubs.push(onSnapshot(collection(db,"participations"), snap=>{
          State.participations = {}; snap.forEach(d=>State.participations[d.id]={...d.data(), id:d.id}); cb();
        }));
        unsubs.push(onSnapshot(collection(db,"results"), snap=>{
          State.results = {}; snap.forEach(d=>State.results[d.id]=d.data()); cb();
        }));
        onUnsub = ()=>unsubs.forEach(u=>u());
        return onUnsub;
      },
      _mountRealtime(){
        // noop; mounted when subscribeAll is called
      }
    };

    const API = {
      async init(){
        try {
          await CloudStore.init();
        } catch(e) {
          console.warn("Cloud init failed, falling back to local", e);
          State.mode = "local";
          LocalStore.init();
        }
        if(State.mode==="local") LocalStore.init();
      },
      signIn: (...a)=> State.mode==="cloud" ? CloudStore.signIn(...a) : LocalStore.signIn(...a),
      signOut: (...a)=> State.mode==="cloud" ? CloudStore.signOut(...a) : LocalStore.signOut(...a),
      createAccount: (...a)=> State.mode==="cloud" ? CloudStore.createAccount(...a) : LocalStore.createAccount(...a),
      seedTeams: (...a)=> State.mode==="cloud" ? CloudStore.seedTeams(...a) : LocalStore.seedTeams(...a),
      updateTeam: (...a)=> State.mode==="cloud" ? CloudStore.updateTeam(...a) : LocalStore.updateTeam(...a),
      addStudent: (...a)=> State.mode==="cloud" ? CloudStore.addStudent(...a) : LocalStore.addStudent(...a),
      removeStudent: (...a)=> State.mode==="cloud" ? CloudStore.removeStudent(...a) : LocalStore.removeStudent(...a),
      addCompetition: (...a)=> State.mode==="cloud" ? CloudStore.addCompetition(...a) : LocalStore.addCompetition(...a),
      removeCompetition: (...a)=> State.mode==="cloud" ? CloudStore.removeCompetition(...a) : LocalStore.removeCompetition(...a),
      addParticipation: (...a)=> State.mode==="cloud" ? CloudStore.addParticipation(...a) : LocalStore.addParticipation(...a),
      updateParticipation: (...a)=> State.mode==="cloud" ? CloudStore.updateParticipation(...a) : LocalStore.updateParticipation(...a),
      removeParticipation: (...a)=> State.mode==="cloud" ? CloudStore.removeParticipation(...a) : LocalStore.removeParticipation(...a),
      saveResults: (...a)=> State.mode==="cloud" ? CloudStore.saveResults(...a) : LocalStore.saveResults(...a),
      subscribeAll: (cb)=> State.mode==="cloud" ? CloudStore.subscribeAll(cb) : LocalStore.subscribeAll(cb),
    };

    // ========= UI BINDINGS =========
    // Populate category selects
    function fillCategorySelects(){
      for(const sel of ["tAddCat","cCat"]){
        const s = $("#"+sel); s.innerHTML=""; for(const c of CATEGORIES){ const o=document.createElement("option"); o.value=c; o.textContent=c; s.appendChild(o); }
      }
    }
    function fillTeamAccountSelect(){
      const s = $("#accTeam"); s.innerHTML=""; for(const t of TEAMS){ const o=document.createElement("option"); o.value=t; o.textContent=t; s.appendChild(o); }
    }
    function fillAttendanceCompSelects(){
      const comps = Object.values(State.competitions).sort((a,b)=>a.name.localeCompare(b.name));
      for(const selId of ["attSelComp","judgeSelComp","postComp"]){
        const s = $("#"+selId); s.innerHTML = "<option value=''>Select...</option>";
        for(const c of comps){ const o=document.createElement("option"); o.value=c.id; o.textContent = `${c.name} — ${c.category}`; s.appendChild(o); }
      }
    }
    function calcTeamTotals(){
      // aggregate points from results + bonuses - penalties
      const teamPoints = {};
      for(const t of TEAMS){ teamPoints[t] = 0; }
      for(const [compId,res] of Object.entries(State.results)){
        const comp = State.competitions[compId]; if(!comp || !res || !res.winners) continue;
        for(const w of res.winners){
          if(!w || !w.participationId || !w.points) continue;
          const part = State.participations[w.participationId]; if(!part) continue;
          teamPoints[part.teamId] = (teamPoints[part.teamId]||0) + Number(w.points||0);
        }
      }
      // apply bonus/penalty
      for(const t of TEAMS){
        const td = State.teams[t]; if(!td) continue;
        teamPoints[t] = (teamPoints[t]||0) + Number(td.bonus||0) - Number(td.penalty||0);
      }
      return teamPoints;
    }
    function recalcKPIs(){
      $("#kpiStudents").textContent = Object.keys(State.students).length;
      $("#kpiComps").textContent = Object.keys(State.competitions).length;
      $("#kpiParts").textContent = Object.keys(State.participations).length;
      // winners feed: show last 10
      const feed = $("#winnersFeed"); feed.innerHTML="";
      const items = [];
      for(const [cid, res] of Object.entries(State.results)){
        const comp = State.competitions[cid];
        if(res && res.winners){ for(const w of res.winners){
          const p = State.participations[w.participationId]; if(!p) continue;
          const names = (p.studentIds||[]).map(sid=>State.students[sid]?.name).filter(Boolean);
          const nameStr = names.join(", ");
          items.push({ ts: w.updatedAt || 0, text: `${comp?.category || ""} • ${comp?.name || ""} — ${nameStr} (${p.teamId}) • ${ordinal(w.place)} • ${w.points} pts` });
        } }
      }
      items.sort((a,b)=>b.ts-a.ts).slice(0,10).forEach(it=>{
        const li=document.createElement("li"); li.textContent = it.text; feed.appendChild(li);
      });
      // top teams
      const totals = calcTeamTotals();
      const tb = $("#tblTopTeams tbody"); tb.innerHTML="";
      Object.entries(totals).sort((a,b)=>b[1]-a[1]).forEach(([team,pts])=>{
        const tr=document.createElement("tr");
        tr.innerHTML = `<td>${team}</td><td class="right">${pts}</td>`;
        tb.appendChild(tr);
      });
    }
    function ordinal(n){ const s=["th","st","nd","rd"], v=n%100; return n+(s[(v-20)%10]||s[v]||s[0]); }

    // -------- TEAM UI ----------
    function setTeamHeader(){
      $("#teamNameHdr").textContent = State.teamId || "";
      const t = State.teams[State.teamId] || {};
      $("#teamLockBadge").textContent = t.locked ? "Locked" : "Open for Editing";
      $("#teamLockBadge").className = "badge " + (t.locked?"warnc":"ok");
    }
    function renderTeamStudents(){
      const tb = $("#tblTeamStudents tbody"); tb.innerHTML="";
      const rows = Object.values(State.students).filter(s=>s.teamId===State.teamId)
        .sort((a,b)=>String(a.chestNo).localeCompare(String(b.chestNo)));
      for(const s of rows){
        const count = Object.values(State.participations).filter(p=> (p.studentIds||[]).includes(s.id)).length;
        const tr=document.createElement("tr");
        tr.innerHTML = `
          <td class="mono">${safe(s.chestNo)}</td>
          <td>${safe(s.name)}</td>
          <td>${safe(s.category)}</td>
          <td>${count}</td>
          <td class="right">
            <button class="danger miniBtn" data-rmstu="${s.id}">Remove</button>
          </td>
        `;
        tb.appendChild(tr);
      }
      $$("#tblTeamStudents [data-rmstu]").forEach(btn=>{
        btn.onclick = async ()=>{
          const t = State.teams[State.teamId]; if(t?.locked) return toast("Team is locked", "warnc");
          if(!confirm("Remove this student?")) return;
          try { await API.removeStudent(btn.dataset.rmstu); toast("Removed","ok"); } catch(e){ toast(e.message,"err"); }
        };
      });
    }
    function fillStudentSelect(){
      const s = $("#selRegStudent"); s.innerHTML = "<option value=''>Select student...</option>";
      const rows = Object.values(State.students).filter(s=>s.teamId===State.teamId)
        .sort((a,b)=>safe(a.name).localeCompare(safe(b.name)));
      for(const st of rows){
        const o=document.createElement("option"); o.value = st.id; o.textContent = `${st.name} — ${st.category} — Chest ${st.chestNo}`;
        s.appendChild(o);
      }
    }
    function showAvailableCompetitionsFor(studentId){
      const box = $("#regCompList"); box.innerHTML="";
      const st = State.students[studentId]; if(!st) { $("#regStuInfo").textContent=""; $("#groupBox").classList.add("hidden"); return; }
      $("#regStuInfo").textContent = `Selected: ${st.name} • ${st.category} • Chest ${st.chestNo}`;
      const comps = Object.values(State.competitions).filter(c => c.category === st.category || c.category === "Popular Zone")
        .sort((a,b)=>a.name.localeCompare(b.name));
      for(const c of comps){
        const teamCount = Object.values(State.participations).filter(p=>p.competitionId===c.id && p.teamId===State.teamId).length;
        const btnText = c.type==="group" ? "Create Group Entry" : "Register";
        const card=document.createElement("div"); card.className="card";
        card.innerHTML = `
          <div class="flex">
            <div>
              <div class="h3">${safe(c.name)}</div>
              <div class="sub">${safe(c.category)} • ${c.type} • Max/team: ${c.maxPerTeam} • Current: ${teamCount}</div>
            </div>
            <span class="space"></span>
            <button class="miniBtn" data-regcomp="${c.id}">${btnText}</button>
          </div>
        `;
        box.appendChild(card);
      }
      // Group helper members
      const groupBox = $("#groupBox");
      groupBox.classList.add("hidden");
      $("#groupMembers").innerHTML = "";
      $$("#regCompList [data-regcomp]").forEach(btn=>{
        btn.onclick = ()=>{
          const comp = State.competitions[btn.dataset.regcomp];
          if(!comp) return;
          if(comp.type==="group"){
            groupBox.classList.remove("hidden");
            // list eligible members
            const wrap = $("#groupMembers"); wrap.innerHTML="";
            const elig = Object.values(State.students).filter(x=> x.teamId===State.teamId && ((comp.category==="Popular Zone") || (x.category===comp.category)));
            // create checkboxes
            for(const m of elig){
              const lab=document.createElement("label");
              lab.className="flex";
              lab.innerHTML = `<input type="checkbox" data-gmem="${m.id}" /> <span>${m.name} — ${m.category} — Chest ${m.chestNo}</span>`;
              wrap.appendChild(lab);
            }
            // add register button
            let regBtn = $("#groupBox .regGroupBtn");
            if(!regBtn){
              regBtn = document.createElement("button");
              regBtn.textContent = "Register Group";
              regBtn.className = "regGroupBtn";
              regBtn.style = "margin-top:8px;";
              $("#groupBox").appendChild(regBtn);
            }
            regBtn.onclick = async ()=>{
              const t = State.teams[State.teamId]; if(t?.locked) return toast("Team is locked", "warnc");
              const members = $$("#groupMembers [data-gmem]:checked").map(x=>x.dataset.gmem);
              if(members.length===0) return toast("Select group members","warnc");
              try{
                await API.addParticipation({
                  competitionId: comp.id,
                  category: comp.category,
                  type: "group",
                  teamId: State.teamId,
                  studentIds: members,
                  groupName: $("#groupName").value.trim() || null,
                  createdAt: Date.now()
                });
                toast("Group registered","ok");
                showAvailableCompetitionsFor(studentId);
              }catch(e){ toast(e.message,"err"); }
            }
          } else {
            // individual
            registerIndividual(studentId, btn.dataset.regcomp);
          }
        };
      });
    }
    async function registerIndividual(studentId, compId){
      const t = State.teams[State.teamId]; if(t?.locked) return toast("Team is locked", "warnc");
      try{
        await API.addParticipation({
          competitionId: compId,
          category: State.competitions[compId].category,
          type: "individual",
          teamId: State.teamId,
          studentIds: [studentId],
          createdAt: Date.now()
        });
        toast("Registered","ok");
      } catch(e){ toast(e.message,"err"); }
    }
    function renderTeamCompetitionEntries(){
      const box = $("#teamCompEntries"); box.innerHTML="";
      const myParts = Object.values(State.participations).filter(p=>p.teamId===State.teamId);
      const byComp = groupBy(myParts, p=>p.competitionId);
      const comps = Object.values(State.competitions).filter(c=>byComp.has(c.id)).sort((a,b)=>a.name.localeCompare(b.name));
      if(comps.length===0){ box.innerHTML = `<div class="muted">No entries yet.</div>`; return; }
      for(const c of comps){
        const list = byComp.get(c.id);
        const card = document.createElement("div"); card.className="card";
        const ul = document.createElement("ul"); ul.className="list";
        for(const p of list){
          const names = (p.studentIds||[]).map(sid=>State.students[sid]?.name || "?").join(", ");
          const att = p.attendance ? `<span class="badge">Present</span>` : `<span class="badge">Not marked</span>`;
          const code = p.codeLetter ? `<span class="badge mono">Code: ${p.codeLetter}</span>` : "";
          const li = document.createElement("li");
          li.innerHTML = `
            <div class="flex">
              <div>${names} ${c.type==="group" && p.groupName? `(<span class="mono">${safe(p.groupName)}</span>)`: ""} — ${att} ${code}</div>
              <span class="space"></span>
              <button class="ghost miniBtn" data-rmp="${p.id}">Cancel</button>
            </div>
          `;
          ul.appendChild(li);
        }
        card.innerHTML = `
          <div class="flex"><div class="h3">${c.name}</div><span class="space"></span><span class="badge">${c.category} • ${c.type}</span></div>
        `;
        card.appendChild(ul);
        box.appendChild(card);
      }
      $$("#teamCompEntries [data-rmp]").forEach(btn=>{
        btn.onclick = async ()=>{
          const t = State.teams[State.teamId]; if(t?.locked) return toast("Team is locked", "warnc");
          if(!confirm("Cancel this entry?")) return;
          try{ await API.removeParticipation(btn.dataset.rmp); toast("Cancelled","ok"); }catch(e){ toast(e.message,"err"); }
        };
      });
    }
    function renderTeamParticipationList(){
      const box = $("#teamParticipationList"); box.innerHTML="";
      // For each student: list competitions
      const myStudents = Object.values(State.students).filter(s=>s.teamId===State.teamId)
        .sort((a,b)=>safe(a.name).localeCompare(safe(b.name)));
      const parts = Object.values(State.participations).filter(p=>p.teamId===State.teamId);
      const partsByStudent = new Map();
      for(const p of parts){
        for(const sid of (p.studentIds||[])){
          if(!partsByStudent.has(sid)) partsByStudent.set(sid, []);
          partsByStudent.get(sid).push(p);
        }
      }
      const table = document.createElement("table"); table.className="table";
      table.innerHTML = `<thead><tr><th>Name</th><th>Chest</th><th>Category</th><th>Competitions</th></tr></thead>`;
      const tb=document.createElement("tbody");
      for(const s of myStudents){
        const list = partsByStudent.get(s.id)||[];
        const comps = list.map(p=> State.competitions[p.competitionId]?.name).filter(Boolean).sort();
        const tr=document.createElement("tr");
        tr.innerHTML = `<td>${safe(s.name)}</td><td class="mono">${safe(s.chestNo)}</td><td>${safe(s.category)}</td><td>${safe(comps.join(", "))}</td>`;
        tb.appendChild(tr);
      }
      table.appendChild(tb); box.appendChild(table);
    }
    function printTeamList(){
      const node = $("#teamParticipationList").cloneNode(true);
      const wrap = $("#printArea"); wrap.innerHTML="";
      const head = document.createElement("div");
      head.innerHTML = `<h2>${State.teamId} — Participation List</h2>`;
      wrap.appendChild(head); wrap.appendChild(node);
      wrap.classList.remove("hidden");
      const win = window.open("", "printWin");
      win.document.write(`<html><head><title>${State.teamId} Participation List</title></head><body>${wrap.innerHTML}</body></html>`);
      win.document.close(); win.focus(); win.print(); win.close();
      wrap.classList.add("hidden");
    }

    // -------- EVENT UI --------
    function renderTeamsTable(){
      const tb = $("#tblTeams tbody"); tb.innerHTML="";
      for(const t of TEAMS){
        const d = State.teams[t] || { locked:false, bonus:0, penalty:0 };
        const tr=document.createElement("tr");
        tr.innerHTML = `
          <td>${t}</td>
          <td>${d.locked? '<span class="badge warnc">Locked</span>' : '<span class="badge ok">Open</span>'}</td>
          <td><input class="mono mini" style="max-width:100px" data-bonus="${t}" type="number" value="${Number(d.bonus||0)}" /></td>
          <td><input class="mono mini" style="max-width:100px" data-penalty="${t}" type="number" value="${Number(d.penalty||0)}" /></td>
          <td class="right">
            <button class="warn miniBtn" data-lock="${t}">${d.locked? 'Unlock':'Lock'}</button>
          </td>
        `;
        tb.appendChild(tr);
      }
      $$("#tblTeams [data-lock]").forEach(btn=>{
        btn.onclick = async ()=>{
          try{ await API.updateTeam(btn.dataset.lock, { locked: !(State.teams[btn.dataset.lock]?.locked) }); toast("Updated","ok"); }catch(e){ toast(e.message,"err"); }
        };
      });
      $$("#tblTeams [data-bonus]").forEach(inp=>{
        inp.onchange = async ()=>{
          try{ await API.updateTeam(inp.dataset.bonus, { bonus: Number(inp.value||0) }); toast("Bonus updated","ok"); }catch(e){ toast(e.message,"err"); }
        };
      });
      $$("#tblTeams [data-penalty]").forEach(inp=>{
        inp.onchange = async ()=>{
          try{ await API.updateTeam(inp.dataset.penalty, { penalty: Number(inp.value||0) }); toast("Penalty updated","ok"); }catch(e){ toast(e.message,"err"); }
        };
      });
    }
    function renderCompetitions(){
      const tb = $("#tblComps tbody"); tb.innerHTML="";
      const rows = Object.values(State.competitions).sort((a,b)=>a.name.localeCompare(b.name));
      for(const c of rows){
        const tr=document.createElement("tr");
        tr.innerHTML = `
          <td>${safe(c.name)}</td>
          <td>${safe(c.category)}</td>
          <td>${safe(c.type)}</td>
          <td>${safe(c.maxPerTeam)}</td>
          <td class="right"><button class="danger miniBtn" data-rmc="${c.id}">Remove</button></td>
        `;
        tb.appendChild(tr);
      }
      $$("#tblComps [data-rmc]").forEach(btn=>{
        btn.onclick = async ()=>{
          if(!confirm("Remove competition and its entries/results?")) return;
          try{ await API.removeCompetition(btn.dataset.rmc); toast("Removed","ok"); }catch(e){ toast(e.message,"err"); }
        };
      });
      fillAttendanceCompSelects();
    }
    function renderAttendance(){
      const cid = $("#attSelComp").value;
      const box = $("#attList"); box.innerHTML="";
      if(!cid){ box.innerHTML = `<div class="muted">Select a competition.</div>`; return; }
      const comp = State.competitions[cid];
      const parts = Object.values(State.participations).filter(p=>p.competitionId===cid);
      if(parts.length===0){ box.innerHTML=`<div class="muted">No registrations yet.</div>`; return; }
      const byTeam = groupBy(parts, p=>p.teamId);
      for(const team of TEAMS){
        const list = byTeam.get(team)||[];
        const card=document.createElement("div"); card.className="card";
        card.innerHTML = `<div class="h3">${team}</div>`;
        const ul=document.createElement("ul"); ul.className="list";
        for(const p of list){
          const names = (p.studentIds||[]).map(sid=> State.students[sid]?.name).filter(Boolean).join(", ");
          const li=document.createElement("li");
          li.innerHTML = `
            <div class="grid grid-4">
              <div>${names} ${p.groupName? `(<span class="mono">${safe(p.groupName)}</span>)`:""}</div>
              <div><label class="mini">Attendance</label>
                <select data-att="${p.id}">
                  <option value="false" ${!p.attendance?'selected':''}>Absent/Not marked</option>
                  <option value="true" ${p.attendance?'selected':''}>Present</option>
                </select>
              </div>
              <div><label class="mini">Code Letter</label>
                <input data-code="${p.id}" value="${safe(p.codeLetter||"")}" placeholder="e.g., A12" />
              </div>
              <div class="right" style="align-self:center;">
                <button class="secondary miniBtn" data-save="${p.id}">Save</button>
              </div>
            </div>
          `;
          ul.appendChild(li);
        }
        card.appendChild(ul); box.appendChild(card);
      }
      $$("#attList [data-save]").forEach(btn=>{
        btn.onclick = async ()=>{
          const pid = btn.dataset.save;
          const att = $("#attList [data-att='"+pid+"']").value==="true";
          const code = $("#attList [data-code='"+pid+"']").value.trim();
          try{ await API.updateParticipation(pid, { attendance: att, codeLetter: code }); toast("Saved","ok"); } catch(e){ toast(e.message,"err"); }
        };
      });
    }
    function renderJudge(){
      const cid = $("#judgeSelComp").value;
      const listBox = $("#judgeList"); listBox.innerHTML="";
      const winnersBox = $("#winnersEditor"); winnersBox.innerHTML="";
      if(!cid) { listBox.innerHTML=`<div class="muted">Select a competition.</div>`; return; }
      const comp = State.competitions[cid];
      const parts = Object.values(State.participations).filter(p=>p.competitionId===cid && p.attendance);
      if(parts.length===0){ listBox.innerHTML=`<div class="muted">No present participants.</div>`; }
      else {
        const table=document.createElement("table"); table.className="table";
        table.innerHTML = `<thead><tr><th>Team</th><th>Participants</th><th>Code</th></tr></thead>`;
        const tb=document.createElement("tbody");
        for(const p of parts){
          const names=(p.studentIds||[]).map(sid=> State.students[sid]?.name).filter(Boolean).join(", ");
          const tr=document.createElement("tr");
          tr.innerHTML = `<td>${p.teamId}</td><td>${names}${p.groupName? ` — <span class="mono">${safe(p.groupName)}</span>`:""}</td><td class="mono">${safe(p.codeLetter||"-")}</td>`;
          tb.appendChild(tr);
        }
        table.appendChild(tb); listBox.appendChild(table);
      }
      // winners editor
      const res = State.results[cid]?.winners || [];
      const places = [1,2,3];
      for(const place of places){
        const row = document.createElement("div"); row.className="card";
        const sel = document.createElement("select"); sel.dataset.winSel=place;
        const noneOpt = document.createElement("option"); noneOpt.value=""; noneOpt.textContent="-- Select participant --"; sel.appendChild(noneOpt);
        for(const p of parts){
          const names=(p.studentIds||[]).map(sid=> State.students[sid]?.name).filter(Boolean).join(", ");
          const o=document.createElement("option"); o.value=p.id; o.textContent = `${names} (${p.teamId}) — Code: ${p.codeLetter||"-"}`;
          sel.appendChild(o);
        }
        // points input
        const pts = document.createElement("input"); pts.type="number"; pts.min="0"; pts.placeholder="Points";
        pts.dataset.winPts=place;
        // prefill from existing results
        const found = res.find(x=>Number(x.place)===place);
        if(found){ sel.value=found.participationId||""; pts.value = Number(found.points||0); }
        row.innerHTML = `<div class="h3">${ordinal(place)} Place</div>`;
        row.appendChild(sel);
        const ptsWrap = document.createElement("div"); ptsWrap.style="margin-top:6px;"; ptsWrap.appendChild(pts);
        row.appendChild(ptsWrap);
        winnersBox.appendChild(row);
      }
    }
    async function saveResults(){
      const cid = $("#judgeSelComp").value; if(!cid) return toast("Select competition","warnc");
      const winners = [];
      for(const place of [1,2,3]){
        const sel = $(`[data-winSel='${place}']`); const pid = sel?.value||"";
        const pts = Number($(`[data-winPts='${place}']`)?.value||0);
        if(pid && pts>=0) winners.push({ place, participationId: pid, points: pts, updatedAt: Date.now() });
      }
      try{
        await API.saveResults(cid, winners);
        $("#judgeMsg").textContent = "Saved.";
        setTimeout(()=>$("#judgeMsg").textContent="", 1500);
        toast("Results saved","ok");
      } catch(e){ toast(e.message,"err"); }
    }
    function renderScoreboards(){
      const totals = calcTeamTotals();
      const tb = $("#tblScoreOverall tbody"); tb.innerHTML="";
      Object.entries(totals).sort((a,b)=>b[1]-a[1]).forEach(([team,pts])=>{
        const tr=document.createElement("tr"); tr.innerHTML = `<td>${team}</td><td class="right">${pts}</td>`; tb.appendChild(tr);
      });
      // category champions
      const champ = $("#catChampions"); champ.innerHTML="";
      for(const cat of CATEGORIES){
        if(cat==="Popular Zone"){
          const note = document.createElement("div"); note.className="note";
          note.textContent = "Popular Zone is open to all categories; points are counted in overall but not shown as a separate champion by default.";
          champ.appendChild(note); continue;
        }
        const ptsByTeam = {};
        for(const t of TEAMS){ ptsByTeam[t]=0; }
        // Sum only for competitions in this category
        for(const [cid,res] of Object.entries(State.results)){
          const comp=State.competitions[cid]; if(!comp || comp.category !== cat) continue;
          for(const w of res.winners||[]){
            const p = State.participations[w.participationId]; if(!p) continue;
            ptsByTeam[p.teamId] += Number(w.points||0);
          }
        }
        const list = Object.entries(ptsByTeam).sort((a,b)=>b[1]-a[1]);
        const card=document.createElement("div"); card.className="card";
        card.innerHTML = `<div class="h3">${cat}</div>`;
        const t=document.createElement("table"); t.className="table";
        const tb2=document.createElement("tbody");
        for(const [team,pts] of list){
          const tr=document.createElement("tr"); tr.innerHTML = `<td>${team}</td><td class="right">${pts}</td>`; tb2.appendChild(tr);
        }
        t.appendChild(tb2); card.appendChild(t); champ.appendChild(card);
      }
      // Winners by category and competition order
      const winnersBox = $("#winnersByCat"); winnersBox.innerHTML="";
      for(const cat of CATEGORIES.filter(c=>c!=="Popular Zone")){
        const wrap=document.createElement("div"); wrap.className="card";
        wrap.innerHTML = `<div class="h3">${cat}</div>`;
        const ul=document.createElement("ul"); ul.className="list";
        // For competitions in category, list winners in order: 1st, 2nd, 3rd
        const comps = Object.values(State.competitions).filter(c=>c.category===cat).sort((a,b)=>a.name.localeCompare(b.name));
        for(const c of comps){
          const res = State.results[c.id]?.winners||[];
          const items = res.slice().sort((a,b)=>a.place-b.place).map(w=>{
            const p = State.participations[w.participationId]; if(!p) return null;
            const names=(p.studentIds||[]).map(sid=>State.students[sid]?.name).filter(Boolean).join(", ");
            return `${names} — ${c.name} — ${ordinal(w.place)} — ${w.points} point${Number(w.points||0)===1?'':'s'}`;
          }).filter(Boolean);
          for(const line of items){
            const li=document.createElement("li"); li.textContent = line; ul.appendChild(li);
          }
        }
        wrap.appendChild(ul); winnersBox.appendChild(wrap);
      }
    }

    // -------- POSTER --------
    let posterImage = null;
    function posterDraw(){
      const canvas = $("#posterCanvas"), ctx = canvas.getContext("2d");
      ctx.clearRect(0,0,canvas.width,canvas.height);
      if(posterImage){
        // Fit to canvas
        const ratio = Math.min(canvas.width/posterImage.width, canvas.height/posterImage.height);
        const w = posterImage.width*ratio, h = posterImage.height*ratio;
        const x = (canvas.width - w)/2, y=(canvas.height - h)/2;
        ctx.drawImage(posterImage, x, y, w, h);
      } else {
        ctx.fillStyle = "#000"; ctx.fillRect(0,0,canvas.width,canvas.height);
      }
      const line1 = $("#postLine1").value; const line2 = $("#postLine2").value; const line3 = $("#postLine3").value;
      const font = $("#postFont").value || "bold 48px Inter";
      const color = $("#postColor").value || "#fff";
      const shadow = $("#postShadow").value || "rgba(0,0,0,0.6)";
      const y1 = Number($("#y1").value||200), y2=Number($("#y2").value||260), y3=Number($("#y3").value||320);
      ctx.font = font; ctx.textAlign="center"; ctx.textBaseline="middle";
      ctx.fillStyle = color;
      ctx.shadowColor = shadow; ctx.shadowBlur = 6; ctx.shadowOffsetX = 2; ctx.shadowOffsetY = 3;
      const cx = canvas.width/2;
      if(line1) ctx.fillText(line1, cx, y1);
      if(line2) ctx.fillText(line2, cx, y2);
      if(line3) ctx.fillText(line3, cx, y3);
      // reset shadow
      ctx.shadowBlur=0; ctx.shadowOffsetX=0; ctx.shadowOffsetY=0;
    }

    // ========= SEARCH =========
    function attachSearch(inputEl, scope){
      inputEl.oninput = ()=>{
        const q = inputEl.value.trim().toLowerCase();
        if(scope==="team"){
          // filter students table
          const rows = $$("#tblTeamStudents tbody tr");
          rows.forEach(r=>{
            const txt = r.textContent.toLowerCase(); r.style.display = txt.includes(q)? "":"none";
          });
          // filter my comps entries
          $$("#teamCompEntries .card").forEach(card=>{
            card.style.display = card.textContent.toLowerCase().includes(q)? "":"none";
          });
        } else {
          // event: filter comps and students and participation lists where visible
          $$("#tblComps tbody tr, #tblTeams tbody tr, #attList .card, #winnersByCat .card, #tblScoreOverall tbody tr").forEach(el=>{
            el.style.display = el.textContent.toLowerCase().includes(q) ? "" : "none";
          });
        }
      };
    }

    // ========= INIT UI =========
    function bindLogin(){
      $("#btnLogin").onclick = async ()=>{
        const roleSel = $("#loginRole").value;
        const email = $("#loginEmail").value.trim();
        const pass = $("#loginPass").value.trim();
        $("#loginMsg").textContent = "";
        try {
          const prof = await API.signIn(email, pass);
          if(roleSel==="team" && prof.role!=="team"){ throw new Error("Not a team account"); }
          if(roleSel==="event" && prof.role!=="event"){ throw new Error("Not an event crew account"); }
          afterLogin(prof);
        } catch(e){
          $("#loginMsg").textContent = e.message;
          toast(e.message, "err");
        }
      };
      $("#btnDemo").onclick = async ()=>{
        $("#loginEmail").value = "qairuwan@felizia";
        $("#loginPass").value = "team123";
        $("#loginRole").value = "team";
        $("#btnLogin").click();
      };
    }
    function tabs(containerSel, tabAttr, onChange){
      const tabs = $$(`${containerSel} .tab`);
      tabs.forEach(t=>{
        t.onclick = ()=>{
          tabs.forEach(x=>x.classList.remove("active")); t.classList.add("active");
          const id = t.dataset[tabAttr];
          $$(`${containerSel.replace("Tab","")} [id^="${containerSel.replace("#", "").replace("Tab","")}"]`).forEach(x=>x.classList.add("hidden"));
          const view = document.getElementById((containerSel.replace("#",""))+"-"+id);
          if(view) view.classList.remove("hidden");
          if(onChange) onChange(id);
        };
      });
    }
    function afterLogin(prof){
      $("#viewLogin").classList.add("hidden");
      API.subscribeAll(()=>{
        if(State.role==="team"){ setTeamHeader(); renderTeamStudents(); fillStudentSelect(); renderTeamCompetitionEntries(); renderTeamParticipationList(); }
        if(State.role==="event"){ recalcKPIs(); renderTeamsTable(); renderCompetitions(); fillAttendanceCompSelects(); renderScoreboards(); }
      });
      if(State.role==="team"){
        $("#viewTeam").classList.remove("hidden");
        tabs("#teamTab","teamTab");
      } else {
        $("#viewEvent").classList.remove("hidden");
        tabs("#eventTab","eventTab",(id)=>{
          if(id==="attendance") renderAttendance();
          if(id==="judge") renderJudge();
          if(id==="scoreboard") renderScoreboards();
        });
      }
    }

    // ========= BIND CONTROLS =========
    function bindControls(){
      // team add student
      $("#btnAddStudent").onclick = async ()=>{
        const team = State.teams[State.teamId]; if(team?.locked) return toast("Team is locked","warnc");
        const chest = $("#tAddChest").value.trim();
        const name = $("#tAddName").value.trim();
        const cat = $("#tAddCat").value;
        if(!chest || !name || !cat) return toast("Fill all fields","warnc");
        try{
          await API.addStudent({ chestNo: chest, name, category: cat, teamId: State.teamId, createdAt: Date.now() });
          $("#tAddChest").value=""; $("#tAddName").value=""; $("#tAddCat").selectedIndex=0;
          toast("Student added","ok");
        } catch(e){ toast(e.message,"err"); }
      };
      $("#selRegStudent").onchange = ()=> showAvailableCompetitionsFor($("#selRegStudent").value);
      $("#btnPrintTeamList").onclick = ()=> printTeamList();
      $("#btnLogoutTeam").onclick = async ()=>{ await API.signOut(); location.reload(); };

      // event: teams
      $("#btnSeedTeams").onclick = async ()=>{ try{ await API.seedTeams(); toast("Teams initialized","ok"); }catch(e){ toast(e.message,"err"); } };
      $("#btnCreateTeamAccount").onclick = async ()=>{
        const teamId = $("#accTeam").value; const email = $("#accEmail").value.trim(); const pass = $("#accPass").value.trim();
        if(!teamId || !email || !pass) return toast("Fill all fields","warnc");
        try{ await API.createAccount({ email, pass, role:"team", teamId }); $("#accMsg").textContent="Created"; toast("Account created","ok"); }catch(e){ $("#accMsg").textContent=e.message; toast(e.message,"err"); }
      };
      $("#btnCreateEventAccount").onclick = async ()=>{
        const email = $("#accEventEmail").value.trim(); const pass = $("#accEventPass").value.trim();
        if(!email || !pass) return toast("Fill all fields","warnc");
        try{ await API.createAccount({ email, pass, role:"event", teamId:null }); $("#accEventMsg").textContent="Created"; toast("Event account created","ok"); }catch(e){ $("#accEventMsg").textContent=e.message; toast(e.message,"err"); }
      };

      // event: competitions
      $("#btnAddComp").onclick = async ()=>{
        const name = $("#cName").value.trim(); const category = $("#cCat").value; const type = $("#cType").value; const maxPerTeam = Number($("#cMaxTeam").value||0);
        if(!name || !category || !type || maxPerTeam<=0) return toast("Fill all fields correctly","warnc");
        try{ await API.addCompetition({ name, category, type, maxPerTeam, createdAt: Date.now() }); $("#cName").value=""; $("#cMaxTeam").value="3"; toast("Competition added","ok"); }catch(e){ toast(e.message,"err"); }
      };

      // attendance
      $("#attSelComp").onchange = renderAttendance;

      // judge panel
      $("#judgeSelComp").onchange = renderJudge;
      $("#btnSaveResults").onclick = saveResults;

      // poster
      $("#postImg").onchange = (e)=>{
        const file = e.target.files?.[0]; if(!file) return;
        const img = new Image(); img.onload = ()=>{ posterImage = img; posterDraw(); }; img.src = URL.createObjectURL(file);
      };
      $("#btnRenderPoster").onclick = ()=> posterDraw();
      $("#btnDownloadPoster").onclick = ()=>{
        const a=document.createElement("a"); a.download="poster.png"; a.href = $("#posterCanvas").toDataURL("image/png"); a.click();
      };
      $("#btnAutofillPoster").onclick = ()=>{
        const cid = $("#postComp").value; const place = Number($("#postPlace").value||1);
        const res = State.results[cid]?.winners||[]; const winner = res.find(x=>Number(x.place)===place);
        if(!winner) return toast("No winner found for that place","warnc");
        const p = State.participations[winner.participationId]; const comp = State.competitions[cid];
        const names=(p.studentIds||[]).map(sid=>State.students[sid]?.name).filter(Boolean).join(", ");
        $("#postLine1").value = names || "";
        $("#postLine2").value = comp?.category || "";
        $("#postLine3").value = `${comp?.name || ""} — ${ordinal(place)}`;
        posterDraw();
      };

      // search
      attachSearch($("#teamSearch"), "team");
      attachSearch($("#eventSearch"), "event");

      // logout
      $("#btnLogoutEvent").onclick = async ()=>{ await API.signOut(); location.reload(); };
    }

    // ========= BOOT =========
    async function boot(){
      fillCategorySelects();
      fillTeamAccountSelect();
      bindLogin();
      bindControls();
      await API.init();
    }
    boot();
  </script>

  <!-- Firestore Security Rules (copy this into Firebase console) -->
  <!--
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    function isSignedIn() { return request.auth != null; }
    function userProfile() {
      return isSignedIn() ? get(/databases/$(database)/documents/profiles/$(request.auth.uid)).data : null;
    }
    function isEventCrew() { return isSignedIn() && userProfile().role == 'event'; }
    function isTeam() { return isSignedIn() && userProfile().role == 'team'; }
    function myTeamId() { return userProfile().teamId; }

    match /profiles/{uid} {
      allow read: if isSignedIn() && (uid == request.auth.uid || isEventCrew());
      allow write: if isEventCrew();
    }
    match /teams/{teamId} {
      allow read: if isSignedIn();
      allow write: if isEventCrew();
    }
    match /students/{id} {
      allow read: if isEventCrew() || (isTeam() && resource.data.teamId == myTeamId());
      allow create: if isEventCrew() || (isTeam() && request.resource.data.teamId == myTeamId() && get(/databases/$(database)/documents/teams/$(myTeamId())).data.locked == false);
      allow update, delete: if isEventCrew() || (isTeam() && resource.data.teamId == myTeamId() && get(/databases/$(database)/documents/teams/$(myTeamId())).data.locked == false);
    }
    match /competitions/{id} {
      allow read: if isSignedIn();
      allow write: if isEventCrew();
    }
    match /participations/{id} {
      allow read: if isEventCrew() || (isTeam() && resource.data.teamId == myTeamId());
      allow create: if isEventCrew() || (isTeam() && request.resource.data.teamId == myTeamId() && get(/databases/$(database)/documents/teams/$(myTeamId())).data.locked == false);
      allow update, delete: if isEventCrew() || (isTeam() && resource.data.teamId == myTeamId() && get(/databases/$(database)/documents/teams/$(myTeamId())).data.locked == false);
    }
    match /results/{compId} {
      allow read: if isSignedIn();
      allow write: if isEventCrew();
    }
  }
}
  -->
</body>
</html>
