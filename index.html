# coppenheim80-sourcd.github.io
Custom Mini Puzzle
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover" />
  <meta name="apple-mobile-web-app-capable" content="yes" />
  <meta name="apple-mobile-web-app-status-bar-style" content="default" />
  <meta name="apple-mobile-web-app-title" content="The Mini" />
  <meta name="mobile-web-app-capable" content="yes" />
  <meta name="theme-color" content="#ffffff" />
  <title>The Mini</title>
  <style>
    :root {
      --bg: #ffffff;
      --text: #121212;
      --muted: #6b7280;
      --border: #121212;
      --cell-border: #bdbdbd;
      --highlight-word: #a7d8ff;
      --highlight-cell: #ffda00;
      --correct: #2e7d32;
      --wrong: #d32f2f;
      --key-bg: #d3d6da;
      --key-active: #9ca3af;
      --clue-bar: #dceeff;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      -webkit-tap-highlight-color: transparent;
      user-select: none;
      -webkit-user-select: none;
      touch-action: manipulation;
    }

    html, body {
      width: 100%;
      height: 100dvh;
      overflow: hidden;
      background: #f3f4f6;
      color: var(--text);
      display: flex;
      justify-content: center;
    }

    .app-shell {
      width: 100%;
      max-width: 480px;
      height: 100dvh;
      background: var(--bg);
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      padding-top: env(safe-area-inset-top, 0px);
      padding-bottom: env(safe-area-inset-bottom, 8px);
      box-shadow: 0 0 24px rgba(0,0,0,0.08);
      position: relative;
    }

    /* Top Bar */
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px 14px;
      border-bottom: 1px solid #e5e7eb;
      flex-shrink: 0;
    }

    .title-left {
      display: flex;
      align-items: baseline;
      gap: 10px;
    }

    h1 {
      font-family: Georgia, "Times New Roman", serif;
      font-size: 1.35rem;
      font-weight: 700;
    }

    .timer {
      font-variant-numeric: tabular-nums;
      font-size: 1rem;
      font-weight: 600;
      color: var(--muted);
    }

    .toolbar {
      display: flex;
      gap: 6px;
      align-items: center;
    }

    button.tool-btn, select.tool-select {
      padding: 6px 10px;
      border-radius: 6px;
      border: 1px solid #d1d5db;
      background: #fff;
      font-size: 0.8rem;
      font-weight: 600;
      color: var(--text);
      cursor: pointer;
    }

    button.tool-btn.primary {
      background: var(--text);
      color: #fff;
      border-color: var(--text);
    }

    /* Center Grid Container */
    .board-area {
      flex: 1;
      display: flex;
       flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 8px 16px;
      min-height: 0;
    }

    .grid {
      width: min(84vw, 44dvh, 360px);
      height: min(84vw, 44dvh, 360px);
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      grid-template-rows: repeat(5, 1fr);
      border: 2.5px solid var(--border);
      background: var(--border);
    }

    .cell {
      position: relative;
      background: #fff;
      border: 0.5px solid var(--cell-border);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: clamp(1.4rem, 5.5vw, 2rem);
      font-weight: 700;
      text-transform: uppercase;
      cursor: pointer;
    }

    .cell.black {
      background: var(--border);
      border-color: var(--border);
    }

    .cell.in-word {
      background: var(--highlight-word);
    }

    .cell.active {
      background: var(--highlight-cell) !important;
    }

    .cell .num {
      position: absolute;
      top: 2px;
      left: 3px;
      font-size: 0.68rem;
      font-weight: 600;
      line-height: 1;
      color: var(--text);
      pointer-events: none;
    }

    .cell .letter {
      margin-top: 4px;
    }

    .cell.wrong .letter {
      color: var(--wrong);
      text-decoration: line-through;
    }

    .cell.revealed .letter {
      color: #1d4ed8;
    }

    .cell.verified::after {
      content: "";
      position: absolute;
      top: 3px;
      right: 3px;
      width: 6px;
      height: 6px;
      border-radius: 50%;
      background: var(--correct);
    }

    /* Active Clue Navigator Bar */
    .clue-nav-bar {
      display: grid;
      grid-template-columns: 44px 1fr 44px;
      align-items: center;
      background: var(--clue-bar);
      border-top: 1px solid #b8dcff;
      border-bottom: 1px solid #b8dcff;
      min-height: 54px;
      flex-shrink: 0;
    }

    .nav-arrow {
      height: 100%;
      background: transparent;
      border: none;
      font-size: 1.5rem;
      font-weight: 700;
      color: var(--text);
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
    }

    .nav-arrow:active {
      background: rgba(0,0,0,0.08);
    }

    .clue-display {
      padding: 6px 8px;
      display: flex;
      align-items: center;
      gap: 8px;
      cursor: pointer;
      height: 100%;
    }

    .clue-badge {
      background: #121212;
      color: #fff;
      font-size: 0.75rem;
      font-weight: 800;
      padding: 3px 6px;
      border-radius: 4px;
      flex-shrink: 0;
    }

    .clue-text {
      font-size: 0.95rem;
      font-weight: 600;
      line-height: 1.25;
      color: var(--text);
    }

    /* On-Screen Touch Keyboard */
    .keyboard {
      padding: 8px 4px 6px;
      background: #eef0f3;
      display: flex;
      flex-direction: column;
      gap: 6px;
      flex-shrink: 0;
    }

    .kb-row {
      display: flex;
      justify-content: center;
      gap: 5px;
      width: 100%;
    }

    .key {
      height: 46px;
      flex: 1;
      max-width: 9.2%;
      border-radius: 6px;
      border: none;
      background: #ffffff;
      box-shadow: 0 1px 2px rgba(0,0,0,0.18);
      font-size: 1.1rem;
      font-weight: 700;
      color: var(--text);
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
    }

    .key.wide {
      max-width: 14.5%;
      flex: 1.5;
      background: #d3d6da;
      font-size: 0.85rem;
      font-weight: 800;
    }

    .key:active, .key.pressed {
      background: var(--key-active);
      transform: translateY(1px);
    }

    /* Modal Overlay for Win or All Clues Drawer */
    .modal-overlay {
      position: absolute;
      inset: 0;
      background: rgba(0,0,0,0.5);
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      z-index: 20;
    }

    .modal-overlay.visible {
      display: flex;
    }

    .modal-card {
      background: #fff;
      width: 100%;
      max-width: 360px;
      border-radius: 14px;
      padding: 22px;
      text-align: center;
      box-shadow: 0 12px 32px rgba(0,0,0,0.22);
      max-height: 82dvh;
      overflow-y: auto;
    }

    .modal-card h2 {
      font-size: 1.4rem;
      margin-bottom: 8px;
    }

    .modal-card p {
      color: var(--muted);
      margin-bottom: 18px;
      font-size: 0.95rem;
    }

    .modal-actions {
      display: flex;
      gap: 10px;
      justify-content: center;
    }

    .modal-actions button {
      padding: 10px 18px;
      border-radius: 8px;
      font-size: 0.95rem;
      font-weight: 700;
      border: 1px solid #d1d5db;
      background: #fff;
      cursor: pointer;
    }

    .modal-actions button.primary {
      background: #121212;
      color: #fff;
      border-color: #121212;
    }

    /* Clues Drawer list inside modal */
    .drawer-lists {
      text-align: left;
      margin-bottom: 16px;
      font-size: 0.88rem;
    }

    .drawer-lists h4 {
      text-transform: uppercase;
      font-size: 0.78rem;
      letter-spacing: 0.05em;
      color: var(--muted);
      margin: 10px 0 4px;
      border-bottom: 1px solid #e5e7eb;
      padding-bottom: 3px;
    }

    .drawer-item {
      padding: 5px 4px;
      border-bottom: 1px solid #f3f4f6;
      cursor: pointer;
    }
  </style>
</head>
<body>

<div class="app-shell">
  <header>
    <div class="title-left">
      <h1>The Mini</h1>
      <span class="timer" id="timer">0:00</span>
    </div>
    <div class="toolbar">
      <select id="templateSelect" class="tool-select" aria-label="Shape">
        <option value="random">Mix</option>
        <option value="0">Stairs</option>
        <option value="1">Corners</option>
        <option value="2">Cut</option>
        <option value="3">5×5 Open</option>
      </select>
      <button class="tool-btn" id="cluesBtn" type="button">Clues</button>
      <button class="tool-btn" id="checkBtn" type="button">Check</button>
      <button class="tool-btn" id="hintBtn" type="button">Hint</button>
      <button class="tool-btn primary" id="newBtn" type="button">New</button>
    </div>
  </header>

  <div class="board-area">
    <div class="grid" id="grid"></div>
  </div>

  <!-- Tap-to-flip Clue Bar with Prev / Next buttons -->
  <div class="clue-nav-bar">
    <button class="nav-arrow" id="prevClueBtn" type="button" aria-label="Previous Clue">‹</button>
    <div class="clue-display" id="clueBannerTap" title="Tap to flip Across/Down">
      <span class="clue-badge" id="bannerNum">1A</span>
      <span class="clue-text" id="bannerText">Generating puzzle...</span>
    </div>
    <button class="nav-arrow" id="nextClueBtn" type="button" aria-label="Next Clue">›</button>
  </div>

  <!-- Custom QWERTY On-Screen Touch Keyboard -->
  <div class="keyboard" id="keyboard">
    <div class="kb-row">
      <button class="key" data-key="Q">Q</button>
      <button class="key" data-key="W">W</button>
      <button class="key" data-key="E">E</button>
      <button class="key" data-key="R">R</button>
      <button class="key" data-key="T">T</button>
      <button class="key" data-key="Y">Y</button>
      <button class="key" data-key="U">U</button>
      <button class="key" data-key="I">I</button>
      <button class="key" data-key="O">O</button>
      <button class="key" data-key="P">P</button>
    </div>
    <div class="kb-row">
      <button class="key" data-key="A">A</button>
      <button class="key" data-key="S">S</button>
      <button class="key" data-key="D">D</button>
      <button class="key" data-key="F">F</button>
      <button class="key" data-key="G">G</button>
      <button class="key" data-key="H">H</button>
      <button class="key" data-key="J">J</button>
      <button class="key" data-key="K">K</button>
      <button class="key" data-key="L">L</button>
    </div>
    <div class="kb-row">
      <button class="key wide" data-key="FLIP" title="Flip Across/Down">A/D ⇄</button>
      <button class="key" data-key="Z">Z</button>
      <button class="key" data-key="X">X</button>
      <button class="key" data-key="C">C</button>
      <button class="key" data-key="V">V</button>
      <button class="key" data-key="B">B</button>
      <button class="key" data-key="N">N</button>
      <button class="key" data-key="M">M</button>
      <button class="key wide" data-key="BACKSPACE" aria-label="Backspace">⌫</button>
    </div>
  </div>

  <!-- Victory Modal -->
  <div class="modal-overlay" id="winModal">
    <div class="modal-card">
      <h2>🎉 Puzzle Solved!</h2>
      <p id="winStatsText">You finished The Mini in 0:45.</p>
      <div class="modal-actions">
        <button id="closeWinBtn" type="button">View Board</button>
        <button class="primary" id="playAgainBtn" type="button">Next Puzzle</button>
      </div>
    </div>
  </div>

  <!-- All Clues Modal Drawer -->
  <div class="modal-overlay" id="cluesModal">
    <div class="modal-card">
      <h2>All Clues</h2>
      <div class="drawer-lists" id="drawerContent"></div>
      <div class="modal-actions">
        <button id="revealAllBtn" type="button">Reveal Solution</button>
        <button class="primary" id="closeCluesBtn" type="button">Close</button>
      </div>
    </div>
  </div>
</div>

<script>
const RAW_DICTIONARY = [
  // --- 5-LETTER HIGH-CROSSABILITY WORDS ---
  ["ROTOR", "Spinning assembly inside a turbine"],
  ["CRUST", "Artisanal loaf's caramelized exterior"],
  ["CRUMB", "Interior hole structure of baked bread"],
  ["FLOUR", "Baker's primary dry ingredient"],
  ["YEAST", "Single-celled leavening agent"],
  ["BRINE", "Salty bath for lacto-fermentation"],
  ["SHALE", "Fine-grained sedimentary rock"],
  ["VALVE", "Flow-regulating pipe fitting"],
  ["GAUGE", "Dial on a pressurized tank"],
  ["LASER", "Coherent optical beam"],
  ["ALLOY", "Metallic solid solution, like brass or steel"],
  ["LATHE", "Machine shop turning tool"],
  ["BEVEL", "Angled edge on a machined plate"],
  ["RIVET", "Heavy-duty metal fastener"],
  ["WELDS", "Fuses metal plates with an arc"],
  ["SPARK", "Ignition gap flash"],
  ["PULSE", "Rhythmic beat or signal spike"],
  ["PHASE", "Distinct state of matter"],
  ["VAPOR", "Gas below its critical temperature"],
  ["STEAM", "Pressurized boiler output"],
  ["SLOPE", "Rise divided by run"],
  ["DRAFT", "Preliminary CAD drawing"],
  ["SCALE", "Drawing ratio, e.g., 1:10"],
  ["LIMIT", "Calculus boundary value"],
  ["PRIME", "Number divisible only by 1 and itself"],
  ["DELTA", "Symbol for a finite increment"],
  ["SIGMA", "Greek letter representing normal stress"],
  ["OMEGA", "Symbol for angular velocity"],
  ["RATIO", "Dimensionless quotient"],
  ["PIVOT", "Fulcrum point"],
  ["LEVER", "Simple machine that multiplies force"],
  ["WEDGE", "Simple machine used for splitting"],
  ["SCREW", "Helical inclined plane fastener"],
  ["WHEEL", "Rotating disk on an axle"],
  ["SHAFT", "Rotating bar transmitting torque"],
  ["AXLES", "Spindles supporting rotating wheels"],
  ["GEARS", "Toothed wheels that alter torque"],
  ["BELTS", "Flexible loops connecting pulleys"],
  ["CHAIN", "Roller drive on a bicycle"],
  ["BRAKE", "Energy-dissipating friction device"],
  ["SPEED", "Magnitude of the velocity vector"],
  ["FORCE", "Mass times acceleration"],
  ["POWER", "Work performed per unit time"],
  ["JOULE", "SI unit of energy"],
  ["TESLA", "SI unit of magnetic flux density"],
  ["FARAD", "SI unit of electrical capacitance"],
  ["WATTS", "Units on a lightbulb package"],
  ["VOLTS", "Electromotive force units"],
  ["DIODE", "One-way semiconductor gate"],
  ["ANODE", "Electrode where oxidation occurs"],
  ["RELAY", "Electrically operated switch"],
  ["LOGIC", "Boolean circuit fundamentals"],
  ["ARRAY", "Indexed data structure"],
  ["STACK", "Last-in, first-out memory structure"],
  ["CACHE", "High-speed processor memory buffer"],
  ["PIXEL", "Smallest addressable screen element"],
  ["TOKEN", "Lexical parser unit"],
  ["NODES", "Intersection points in a finite element mesh"],
  ["TRUSS", "Triangulated structural framework"],
  ["STRUT", "Structural member resisting compression"],
  ["BEAMS", "Horizontal members resisting bending"],
  ["LOADS", "External forces applied to a structure"],
  ["SHEAR", "Sliding stress parallel to a cross-section"],
  ["YIELD", "Onset of permanent plastic deformation"],
  ["CREEP", "Slow deformation under high-temperature stress"],
  ["CRACK", "Fracture mechanics flaw"],
  ["GRAIN", "Crystalline region in a metal"],
  ["STEEL", "Iron-carbon structural alloy"],
  ["BRASS", "Copper-zinc acoustic and valve alloy"],
  ["INGOT", "Cast oblong block of purified metal"],
  ["SMELT", "Extract metal from ore using heat"],
  ["SLAGS", "Vitreous byproducts of ore smelting"],
  ["FORGE", "Shape heated metal via compressive blows"],
  ["ANVIL", "Blacksmith's heavy iron block"],
  ["TONGS", "Gripping tool for hot metalwork"],
  ["RESIN", "Polymer matrix in carbon fiber"],
  ["GLASS", "Amorphous silicate solid"],
  ["LITER", "Metric volume of 1,000 cubic centimeters"],
  ["METER", "Base SI unit of length"],
  ["GRAMS", "Metric mass units on a kitchen scale"],
  ["OUNCE", "One-sixteenth of a pound"],
  ["CARAT", "200-milligram gemstone mass unit"],
  ["SONAR", "Acoustic underwater ranging system"],
  ["RADAR", "Radio-wave detection and ranging system"],
  ["ORBIT", "Keplerian elliptical trajectory"],
  ["COMET", "Icy solar system body with a tail"],
  ["SOLAR", "Powered by the sun"],
  ["LUNAR", "Relating to Earth's natural satellite"],
  ["STARS", "Main-sequence fusion furnaces"],
  ["EARTH", "Third rock from the sun"],
  ["OCEAN", "71% of Earth's surface"],
  ["TIDES", "Gravitational sea-level oscillations"],
  ["WAVES", "Oscillations that transfer energy"],
  ["WINDS", "Pressure-gradient atmospheric flows"],
  ["STORM", "Low-pressure meteorological disturbance"],
  ["CLOUD", "Visible aerosol of water droplets"],
  ["FROST", "Sub-freezing vapor deposition"],
  ["GLAZE", "Smooth, glossy coating"],
  ["SPICE", "Aromatic culinary seasoning"],
  ["HERBS", "Leafy green flavorings like basil or thyme"],
  ["SAUCE", "Liquid culinary condiment"],
  ["ROAST", "Cook with dry oven heat"],
  ["BAKES", "Cooks in an enclosed oven"],
  ["KNEAD", "Work dough to develop gluten"],
  ["PROOF", "Final dough rise before baking"],
  ["SCORE", "Slash bread dough with a lame"],
  ["BAGEL", "Boiled-and-baked ring roll"],
  ["TOAST", "Browned bread slice"],
  ["PASTA", "Extruded durum wheat semolina dough"],
  ["OLIVE", "Mediterranean oil fruit"],
  ["LEMON", "Tart citric acid source"],
  ["BERRY", "Small pulpy fruit"],
  ["MELON", "Cantaloupe or honeydew"],
  ["PEACH", "Fuzzy stone fruit"],
  ["GRAPE", "Winemaker's raw material"],
  ["CIDER", "Pressed orchard beverage"],
  ["LAGER", "Cold-fermented crisp beer"],
  ["STOUT", "Dark roasted-barley ale"],
  ["WATER", "Universal polar solvent"],
  ["TIGER", "Striped apex predator"],
  ["EAGLE", "High-soaring raptor"],
  ["SHARK", "Cartilaginous ocean predator"],
  ["WHALE", "Largest marine mammal"],
  ["SNAKE", "Limbless reptile"],
  ["CRANE", "Tall construction hoist"],
  ["HERON", "Long-legged marsh bird"],
  ["RAVEN", "Clever corvid bird"],
  ["ROBIN", "Red-breasted songbird"],
  ["TRAIN", "Locomotive and cars"],
  ["PLANE", "Fixed-wing aircraft"],
  ["CANOE", "Paddled lightweight boat"],
  ["CABIN", "Woodland getaway retreat"],
  ["TRAIL", "Backcountry footpath"],
  ["RIDGE", "Elevated mountain crest"],
  ["CLIFF", "Sheer rock face"],
  ["SHORE", "Where land meets sea"],
  ["BEACH", "Sandy coastal stretch"],
  ["DUNES", "Wind-sculpted sand hills"],
  ["OASIS", "Fertile desert spring"],
  ["TREES", "Binary search data structures"],
  ["ROOTS", "Polynomial zeros"],
  ["SEEDS", "Random number generator initializers"],
  ["STEMS", "Wineglass supports"],
  ["THORN", "Rosebush defense"],
  ["CHESS", "64-square strategy game"],
  ["BOARD", "Tabletop gaming surface"],
  ["CARDS", "Deck of 52"],
  ["POKER", "Texas Hold'em game"],
  ["PIANO", "88-key percussion instrument"],
  ["TEMPO", "Sustained threshold running pace"],
  ["NOTES", "Musical pitches"],
  ["STAGE", "Single step in a multi-rotor compressor"],
  ["BLADE", "Airfoil-shaped rotor vane"],
  ["VANES", "Flow-directing diffuser foils"],
  ["SEALS", "Leakage-preventing shaft barriers"],
  ["PORTS", "Fluid intake or exhaust openings"],
  ["DUCTS", "Sheet-metal air passages"],
  ["PIPES", "Tubular fluid conduits"],
  ["TUBES", "Hollow cylindrical conduits"],
  ["TANKS", "Pressurized storage vessels"],
  ["PUMPS", "Machines that add head to liquids"],
  ["MOTOR", "Electrical-to-mechanical prime mover"],
  ["DRIVE", "Power transmission system"],
  ["ALIBI", "Courtroom excuse"],
  ["REBEL", "Defy established convention"],
  ["TALES", "Imaginative stories"],
  ["PALES", "Loses color in comparison"],
  ["SPARE", "Extra tire in the trunk"],
  ["STARE", "Fixed, unblinking look"],
  ["SLATE", "Metamorphic roofing rock"],
  ["CRATE", "Slatted wooden shipping box"],
  ["PLATE", "Flat structural metal sheet"],
  ["GRATE", "Fireplace iron bars"],
  ["TRACE", "Tiny, barely measurable amount"],
  ["SPACE", "Three-dimensional continuum"],
  ["BRACE", "Diagonal structural stiffener"],
  ["GRACE", "Effortless elegance"],
  ["PLACE", "Position in a sequence"],
  ["SLICE", "Thin cross-sectional cut"],
  ["PRICE", "Market clearing cost"],
  ["STONE", "Fourteen pounds, in Britain"],
  ["ATONE", "Make amends"],
  ["CLONE", "Exact genetic duplicate"],
  ["DRONE", "Unmanned quadcopter"],
  ["PRONE", "Lying flat on one's chest"],
  ["SHONE", "Glowed brightly"],
  ["TONES", "Pure acoustic frequencies"],
  ["ZONES", "Heart-rate training brackets"],
  ["CONES", "Autocross course markers"],
  ["BONES", "Skeletal struts"],
  ["LANES", "Running track divisions"],
  ["PANES", "Window glass sheets"],
  ["SANER", "More level-headed"],
  ["NEARS", "Approaches asymptotically"],
  ["EARNS", "Brings in via hard work"],
  ["SNARE", "Percussion drum with rattling wires"],
  ["ARENA", "Enclosed sports stadium"],
  ["AREAS", "Cross-sectional surface measures"],
  ["ERASE", "Wipe from memory"],
  ["RATES", "Derivatives with respect to time"],
  ["TEARS", "Propagating tensile rips"],
  ["TARES", "Zeroes out a digital scale"],
  ["ASTER", "Star-shaped autumn flower"],
  ["STEER", "Control lateral vehicle direction"],
  ["RESET", "Return a circuit to its initial state"],
  ["ESTER", "Fragrant organic compound"],
  ["ALERT", "Watchful and ready"],
  ["ALTER", "Modify a CAD dimension"],
  ["LATER", "After the current iteration"],
  ["AISLE", "Theater walkway"],
  ["ALIEN", "Extraterrestrial visitor"],
  ["ALINE", "Bring into straight adjustment"],
  ["ARISE", "Come into view"],
  ["RAISE", "Lift to a higher elevation"],
  ["ALONE", "Solo"],
  ["AVOID", "Steer clear of"],
  ["AWAIT", "Wait on an asynchronous promise"],
  ["AWAKE", "Not sleeping"],
  ["AWARE", "Cognizant"],
  ["BASTE", "Moisten roasting meat"],
  ["BEAST", "Formidable machine"],
  ["BEATS", "Acoustic interference pulsations"],
  ["BETAS", "Early software test releases"],
  ["CATER", "Provide food for an event"],
  ["REACT", "Undergo a chemical change"],
  ["CARTE", "À la ___ menu"],
  ["CLEAR", "Reset the display"],
  ["CLEAT", "Cycling shoe pedal clip"],
  ["DEALT", "Distributed playing cards"],
  ["EARLY", "Ahead of schedule"],
  ["ELATE", "Fill with joy"],
  ["EMAIL", "Inbox message"],
  ["ENTER", "Return key label"],
  ["EQUAL", "Balanced on both sides"],
  ["EVENT", "State-machine trigger"],
  ["EXTRA", "Additional margin"],
  ["FALSE", "Boolean 0"],
  ["FEAST", "Celebratory banquet"],
  ["HEART", "Cardiovascular pump"],
  ["HEATS", "Qualifying track races"],
  ["HATES", "Detests"],
  ["HASTE", "Speed that makes waste"],
  ["IDEAL", "Carnot cycle benchmark"],
  ["IMAGE", "Optical lens projection"],
  ["INERT", "Chemically non-reactive, like argon"],
  ["INTER", "Prefix meaning between"],
  ["IRATE", "Furious"],
  ["ITEMS", "Array elements"],
  ["TIMES", "Multiplication operator"],
  ["MITES", "Tiny arachnids"],
  ["EMITS", "Radiates photons"],
  ["LEAST", "Method of ___ squares"],
  ["STALE", "Past peak freshness"],
  ["STEAL", "Take covertly"],
  ["TEALS", "Blue-green duck shades"],
  ["LEAVE", "Depart"],
  ["MEDIA", "Transmission channels"],
  ["METAL", "Ductile conductive solid"],
  ["NOISE", "Unwanted high-frequency static"],
  ["OPERA", "Puccini stage work"],
  ["ORDER", "Highest derivative in a diff-eq"],
  ["OTHER", "Alternative option"],
  ["OUTER", "External boundary"],
  ["ROUTE", "Navigation path"],
  ["PANEL", "Solar array module"],
  ["PEARL", "Oyster gem"],
  ["PEDAL", "Throttle or brake foot lever"],
  ["PLEAD", "Argue in court"],
  ["TREAD", "Tire rubber contact pattern"],
  ["TRADE", "Exchange goods"],
  ["RATED", "Nameplate capacity"],
  ["DARTS", "Pub throwing game"],
  ["SMART", "Self-monitoring and adaptive"],
  ["START", "Green flag signal"],
  ["TARTS", "Fruit pastry shells"],
  ["STATE", "Thermodynamic condition"],
  ["TASTE", "Sample a ferment"],
  ["TEASE", "Gently mock"],
  ["SATED", "Fully satisfied"],
  ["DATES", "Calendar entries"],
  ["STEAD", "In ___ of (replacing)"],
  ["SWEAT", "Evaporative cooling"],
  ["TREAT", "Heat-___ (temper metal)"],
  ["TITLE", "Drawing block header"],
  ["TOTAL", "Grand sum"],
  ["TRIAL", "Experimental test run"],
  ["ULTRA", "Beyond the standard range"],
  ["UNDER", "Below the threshold"],
  ["UNITE", "Bring together"],
  ["UNTIE", "Loosen a knot"],
  ["UPPER", "Higher bound"],
  ["URBAN", "City-centered"],
  ["USAGE", "Consumption rate"],
  ["USUAL", "Standard practice"],
  ["UTTER", "Complete and total"],
  ["VALID", "Meeting all design constraints"],
  ["VALUE", "Scalar magnitude"],
  ["VIDEO", "Moving picture stream"],
  ["VITAL", "Critical to operation"],
  ["VOCAL", "Spoken aloud"],
  ["VOICE", "Acoustic speech signal"],
  ["VOTER", "Ballot caster"],
  ["WASTE", "Rejected scrap heat"],
  ["WATCH", "GPS running wearable"],
  ["WEARY", "Fatigued"],
  ["WEAVE", "Interlace carbon fiber tows"],
  ["WRITE", "Commit data to disk"],
  ["WRIST", "Watch placement joint"],
  ["YEARN", "Long wistfully"],

  // --- 4-LETTER HIGH-CROSSABILITY WORDS ---
  ["SPAR", "Main wing carry-through beam"],
  ["STAR", "Fusion-powered celestial body"],
  ["SILO", "Cylindrical grain or missile tower"],
  ["ROIL", "Stir up turbulent sediment"],
  ["GEAR", "Toothed transmission wheel"],
  ["BEAR", "Carry a structural load"],
  ["BEAM", "Cantilevered structural element"],
  ["SEAM", "Welded joint line"],
  ["SEAL", "Labyrinth or mechanical shaft barrier"],
  ["REAL", "Non-imaginary number component"],
  ["REAM", "Precision-finish a drilled hole"],
  ["TEAM", "Collaborative project group"],
  ["TERM", "Part of a polynomial expression"],
  ["PEAK", "Maximum value on a curve"],
  ["LEAK", "Unwanted pressure vessel escape"],
  ["LEAD", "Spiral advance per single screw turn"],
  ["LOAD", "Applied force or moment"],
  ["ROAD", "Paved highway"],
  ["ROAR", "Rocket booster sound"],
  ["SOAR", "Ride thermal updrafts"],
  ["SOUR", "Lacto-fermented flavor profile"],
  ["POUR", "Cast molten metal into a mold"],
  ["FOUR", "Two squared"],
  ["FOIL", "Aerodynamic wing section"],
  ["COIL", "Helical inductor winding"],
  ["SOIL", "Geotechnical foundation medium"],
  ["BOIL", "Nucleate phase transition"],
  ["BOLT", "Threaded hex-head fastener"],
  ["VOLT", "Joule per coulomb"],
  ["JOLT", "Rate of change of acceleration"],
  ["MALT", "Germinated grain for brewing"],
  ["SALT", "Essential sourdough mineral"],
  ["HALT", "Stop execution"],
  ["HALO", "Circular optical ring"],
  ["HALF", "Fifty percent"],
  ["CALF", "Lower leg running muscle"],
  ["CALL", "Invoke a subroutine"],
  ["WALL", "Boundary layer surface"],
  ["WELL", "Potential energy minimum"],
  ["WELD", "Join metals via coalescence"],
  ["HELD", "Clamped in a fixture"],
  ["HEAD", "Total fluid energy per unit weight"],
  ["HEAT", "Thermal energy in transit"],
  ["NEAT", "Undiluted, at the bar"],
  ["NEAR", "Close in proximity"],
  ["TEAR", "Tensile failure mode"],
  ["TART", "Sharp and acidic"],
  ["PART", "Single CAD component"],
  ["PORT", "Valve opening"],
  ["SORT", "Order an array"],
  ["FORT", "Defensive stronghold"],
  ["FORM", "Sheet-metal stamping die"],
  ["FOAM", "Cellular lightweight core"],
  ["ROAM", "Wander freely"],
  ["FLOW", "Fluid motion"],
  ["SLOW", "Creeping Reynolds regime"],
  ["SLOT", "Keyway groove in a shaft"],
  ["PLOT", "Graph y versus x"],
  ["PLAN", "Top-down orthographic view"],
  ["PLAY", "Backlash clearance between gears"],
  ["CLAY", "Plastic ceramic earth"],
  ["CLAD", "Bonded with a metal layer"],
  ["GLAD", "Pleased"],
  ["GOLD", "Highly conductive noble metal"],
  ["COLD", "Cryogenic temperature regime"],
  ["CORD", "Braided tensile line"],
  ["CORE", "Stator lamination stack"],
  ["CONE", "Supersonic shockwave shape"],
  ["TONE", "Pure sine-wave sound"],
  ["ZONE", "Region on a phase diagram"],
  ["SINK", "Thermal dissipation reservoir"],
  ["LINK", "Four-bar mechanism bar"],
  ["LINE", "One-dimensional figure"],
  ["LIME", "Calcium oxide mineral"],
  ["TIME", "Independent variable t"],
  ["TIDE", "Lunar ocean swell"],
  ["SIDE", "Polygon edge"],
  ["SITE", "Construction location"],
  ["BITE", "Thread engagement depth"],
  ["BITS", "Binary digits"],
  ["BINS", "Histogram intervals"],
  ["FINS", "Heat-transfer surfaces"],
  ["FINE", "High-mesh-density FEA setting"],
  ["VINE", "Vineyard climber"],
  ["VANE", "Aerodynamic turning blade"],
  ["LANE", "Autocross cone corridor"],
  ["LAME", "Baker's razor for scoring dough"],
  ["LATE", "Behind schedule"],
  ["RATE", "Time derivative"],
  ["GATE", "Logic circuit block"],
  ["GALE", "Strong coastal wind"],
  ["PALE", "Light-colored ale style"],
  ["POLE", "Transfer function denominator root"],
  ["PORE", "Microscopic void in sintered metal"],
  ["PURE", "Single-component substance"],
  ["CURE", "Cross-link a polymer"],
  ["TUBE", "Shell-and-___ heat exchanger"],
  ["TUNE", "Adjust PID controller gains"],
  ["DUNE", "Coastal sand ridge"],
  ["DONE", "Fully baked"],
  ["DATA", "Empirical measurements"],
  ["DATE", "Calendar timestamp"],
  ["DART", "Feathered pub projectile"],
  ["DARK", "Absorbing visible light"],
  ["PARK", "Lock the transmission"],
  ["PACT", "Formal treaty"],
  ["FACT", "Verified observation"],
  ["FAST", "High-Mach regime"],
  ["CAST", "Pour metal into a mold"],
  ["CASE", "Outer compressor housing"],
  ["BASE", "Logarithm radix"],
  ["BASS", "Low-frequency audio range"],
  ["MASS", "Measure of translational inertia"],
  ["MAST", "Sailboat spar"],
  ["MESH", "Finite element grid"],
  ["MATH", "Language of engineering"],
  ["PATH", "Line integral trajectory"],
  ["BATH", "Quenching oil tank"],
  ["BARK", "Tree's outer layer"],
  ["MARK", "Calibration scribed line"],
  ["MARS", "Fourth planet from the sun"],
  ["CARS", "Passenger vehicles"],
  ["CART", "Rolling shop utility table"],
  ["CARD", "Punched early-computing medium"],
  ["HARD", "Resistant to Rockwell indentation"],
  ["HAND", "Pressure gauge pointer"],
  ["SAND", "Silica casting mold aggregate"],
  ["SANE", "Rational and sound"],
  ["SALE", "Discounted offering"],
  ["SOLE", "Running shoe bottom assembly"],
  ["SOLO", "Unassisted flight"],
  ["SODA", "Fizzy carbonated drink"],
  ["SOFA", "Living room couch"],
  ["SOFT", "Low-durometer elastomer rating"],
  ["LOFT", "3D CAD blend between sections"],
  ["LIFT", "Force perpendicular to freestream"],
  ["LIFE", "Fatigue cycle endurance"],
  ["FILE", "Machinist's deburring tool"],
  ["FILL", "Crosshatch a 2D drawing section"],
  ["MILL", "Rotary cutting machine"],
  ["MILE", "5,280 feet"],
  ["MILD", "Low-carbon structural steel type"],
  ["MOLD", "Injection cavity block"],
  ["MOLE", "Avogadro's number of particles"],
  ["MODE", "Natural vibration eigenshape"],
  ["NODE", "Zero-amplitude standing wave point"],
  ["NOTE", "Drawing callout specification"],
  ["NONE", "Zero quantity"],
  ["NOSE", "Leading-edge stagnation region"],
  ["HOSE", "Flexible hydraulic line"],
  ["HOST", "Main server machine"],
  ["POST", "Vertical structural column"],
  ["COST", "Objective function to minimize"],
  ["COAT", "Anodized surface layer"],
  ["COAL", "Carbonaceous fossil fuel"],
  ["GOAL", "Target race finish time"],
  ["GOAT", "All-time greatest"],
  ["BOAT", "Displacement hull vessel"],
  ["MOAT", "Castle water trench"],
  ["MEAT", "Heart of the matter"],
  ["MEAN", "Arithmetic average"],
  ["LEAN", "Excess-oxygen fuel mixture"],
  ["READ", "Sample a sensor register"],
  ["REED", "Vibrating strip in a valve"],
  ["SEED", "Crystal nucleation starter"],
  ["SEEK", "Disk head track search"],
  ["WEEK", "Seven-day training microcycle"],
  ["WEAK", "Low-stiffness"],
  ["WEAR", "Tribological surface loss"],
  ["YEAR", "One orbital period of Earth"],
  ["ZERO", "Root of an equation"],
  ["AERO", "Prefix relating to flight"],
  ["AREA", "Integral under a curve"],
  ["ARCS", "Circular geometry segments"],
  ["ARCH", "Compression masonry span"],
  ["INCH", "25.4 millimeters"],
  ["IONS", "Charged atomic species"],
  ["IRON", "Ferrous base metal"],
  ["ICON", "Desktop symbol"],
  ["ECHO", "Reflected acoustic wave"],
  ["ETCH", "Reveal metal grain with acid"],
  ["EACH", "Per unit item"],
  ["EASY", "Recovery run pace"],
  ["EAST", "Sunrise azimuth"],
  ["TEST", "Experimental validation run"],
  ["NEXT", "Subsequent iteration"],
  ["NEST", "Pack parts on a laser sheet"],
  ["WEST", "Sunset direction"],
  ["BEST", "Global optimum"],
  ["REST", "Static equilibrium state"],
  ["RUST", "Hydrated iron oxide"],
  ["RUSH", "Sudden flow surge"],
  ["BUSH", "Sleeve bearing liner"],
  ["PUSH", "Apply compressive force"],
  ["PUMP", "Centrifugal fluid mover"],
  ["DUMP", "Vent pressure rapidly"],
  ["DAMP", "Dissipate vibrational energy"],
  ["LAMP", "Illumination source"],
  ["RAMP", "Linearly increasing input"],
  ["CAMP", "Pitch a tent in Big Sur"],
  ["ABLE", "Capable"],
  ["ACID", "Low-pH proton donor"],
  ["ACRE", "43,560 square feet"],
  ["AGED", "Artificially heat-treated"],
  ["AIDE", "Key assistant"],
  ["ALES", "Taproom pours"],
  ["ALOE", "Soothing succulent"],
  ["ALSO", "In addition"],
  ["ALTO", "Choir voice below soprano"],
  ["AMID", "Surrounded by"],
  ["ANTE", "Poker pot starter"],
  ["ANTS", "Colony insects"],
  ["APEX", "Cornering clipping point"],
  ["ARID", "Bone-dry"],
  ["ARMS", "Cantilevered lever members"],
  ["ATOM", "Basic unit of matter"],
  ["AUTO", "Self-regulating mode"],
  ["AVID", "Enthusiastic"],
  ["AXIS", "Centerline of rotation"],
  ["AXLE", "Wheel-supporting shaft"],
  ["BAKE", "Harden in an oven"],
  ["BALL", "Spherical bearing element"],
  ["BAND", "Frequency pass range"],
  ["BANK", "Superelevated track turn"],
  ["BARE", "Uninsulated wire"],
  ["BARS", "100-kPa pressure units"],
  ["BEAD", "Weld filler pass"],
  ["BEAN", "Espresso seed"],
  ["BEAT", "Interference oscillation"],
  ["BEDS", "Machine tool base castings"],
  ["BEER", "Fermented malt beverage"],
  ["BEET", "Red root used for kvass"],
  ["BELL", "Gaussian curve shape"],
  ["BELT", "Timing drive loop"],
  ["BEND", "Sheet-metal brake operation"],
  ["BENT", "Deflected"],
  ["BETA", "System test release"],
  ["BIAS", "DC offset voltage"],
  ["BIKE", "Two-wheeled vehicle"],
  ["BILL", "___ of materials (BOM)"],
  ["BIND", "Seize up"],
  ["BLUE", "Machinist's spotting dye"],
  ["BODY", "Free-___ diagram"],
  ["BOND", "Atomic link"],
  ["BONE", "Orthopedic strut"],
  ["BOOK", "Reference manual"],
  ["BOOM", "Sonic shockwave clap"],
  ["BORE", "Internal cylinder diameter"],
  ["BOSS", "Cylindrical casting feature"],
  ["BOWL", "Dough mixing vessel"],
  ["BREW", "Ferment beer"],
  ["BULK", "___ fermentation"],
  ["BURN", "Combustion process"],
  ["BURR", "Rough machined metal edge"],
  ["CAGE", "Ball bearing retainer"],
  ["CALM", "Beaufort scale zero"],
  ["CAMS", "Lobed valve actuators"],
  ["CAPE", "Coastal promontory"],
  ["CARE", "Due diligence"],
  ["CASK", "Oak aging barrel"],
  ["CATS", "Ava and Polly, e.g."],
  ["CELL", "Battery galvanic unit"],
  ["CHIP", "Swarf cut by a lathe tool"],
  ["CITY", "___ to the Sea Half Marathon"],
  ["CLAP", "Sharp acoustic impulse"],
  ["CLIP", "Retaining circlip fastener"],
  ["CLUE", "Crossword hint"],
  ["CODE", "ASME pressure vessel standard"],
  ["COGS", "Gear teeth"],
  ["COKE", "Carbon steelmaking fuel"],
  ["COLE", "Cabbage cultivar"],
  ["COOL", "Remove sensible heat"],
  ["COPE", "Top half of a sand-casting flask"],
  ["CORK", "Wine bottle stopper"],
  ["COVE", "Sheltered coastal bay"],
  ["CRAB", "Dungeness crustacean"],
  ["CRAM", "Study intensively"],
  ["CREW", "Rowing team"],
  ["CURL", "Vector cross-product operator"],
  ["CUTS", "Machining passes"],

  // --- 3-LETTER HIGH-CROSSABILITY WORDS ---
  ["RPM", "Tachometer shaft speed units"],
  ["PSI", "Imperial pressure gauge units"],
  ["BAR", "100 kilopascals of pressure"],
  ["OHM", "Unit of electrical resistance"],
  ["AMP", "Coulomb per second"],
  ["ARC", "Welding plasma column"],
  ["CAM", "Eccentric lobe driving a follower"],
  ["COG", "Gear tooth"],
  ["DIE", "Extrusion or threading tool"],
  ["JIG", "Workpiece-guiding device"],
  ["PIN", "Clevis shear fastener"],
  ["ROD", "Piston connecting link"],
  ["NUT", "Internally threaded fastener"],
  ["KEY", "Shaft-to-hub torque insert"],
  ["HUB", "Central boss of an impeller"],
  ["RIM", "Outer wheel perimeter"],
  ["RIB", "Thin stiffening casting web"],
  ["FIN", "Heat sink blade"],
  ["JET", "High-velocity nozzle efflux"],
  ["GAS", "Compressible working fluid"],
  ["OIL", "Bearing lubricant"],
  ["AIR", "78% nitrogen mixture"],
  ["ICE", "Crystalline water"],
  ["ORE", "Metal-bearing rock"],
  ["TIN", "Solder alloy component"],
  ["RAY", "Light path"],
  ["ION", "Charged atom"],
  ["NET", "Resultant force vector"],
  ["SUM", "Sigma notation result"],
  ["SIN", "Opposite over hypotenuse"],
  ["COS", "Adjacent over hypotenuse"],
  ["TAN", "Slope of the angle"],
  ["LOG", "Inverse of exponentiation"],
  ["MAX", "Zero-derivative peak"],
  ["MIN", "Zero-derivative trough"],
  ["BIT", "Binary 0 or 1"],
  ["RAM", "Volatile system memory"],
  ["CPU", "Microprocessor core"],
  ["CAD", "SolidWorks domain"],
  ["FEA", "Mesh-based structural simulation"],
  ["RYE", "Tangy bread grain"],
  ["OAT", "Porridge grain"],
  ["ALE", "Top-fermented brew"],
  ["IPA", "Hoppy craft beer letters"],
  ["TEA", "Steeped leaf infusion"],
  ["PAN", "Sheet-metal baking tray"],
  ["POT", "Simmering vessel"],
  ["LID", "Pressure vessel cover"],
  ["JAR", "Glass fermentation vessel"],
  ["RUN", "Tempo road workout"],
  ["LAP", "400-meter track circuit"],
  ["PAR", "Disc golf hole benchmark"],
  ["ACE", "Disc golf hole-in-one"],
  ["TEE", "First shot launch pad"],
  ["CAT", "Orange tabby pet"],
  ["DOG", "Loyal canine"],
  ["OWL", "Nocturnal raptor"],
  ["JAY", "Crested blue bird"],
  ["SEA", "Coastal salt water"],
  ["BAY", "San Luis Obispo inlet"],
  ["SKY", "Atmosphere overhead"],
  ["SUN", "G-type main-sequence star"],
  ["ERA", "Geologic time division"],
  ["AGE", "Radiometric dating result"],
  ["ACT", "Take action"],
  ["AIM", "Point toward a target"],
  ["ART", "Craftsmanship"],
  ["ASK", "Query"],
  ["AID", "Assistance"],
  ["ADD", "Sum together"],
  ["ARM", "Moment lever length"],
  ["END", "Boundary condition point"],
  ["EAR", "Lifted crust ridge on a scored loaf"],
  ["EAT", "Enjoy a meal"],
  ["ERR", "Deviate from true value"],
  ["GAP", "Rotor tip-to-shroud clearance"],
  ["HIT", "Achieve target spec"],
  ["HOT", "High-enthalpy state"],
  ["LOW", "Suction pressure side"],
  ["MAP", "Compressor performance chart"],
  ["MIX", "Combine reactants"],
  ["NEW", "Freshly initialized"],
  ["NOW", "At t = 0"],
  ["ODD", "Not divisible by two"],
  ["OFF", "Open-circuit state"],
  ["OLD", "Legacy design"],
  ["ONE", "Multiplicative identity"],
  ["OUT", "Discharge port direction"],
  ["OWN", "Possess"],
  ["PAD", "Tilting-___ thrust bearing"],
  ["PEG", "Alignment dowel"],
  ["PEN", "Plotter stylus"],
  ["PIT", "Corrosion surface cavity"],
  ["PLY", "Composite laminate layer"],
  ["PRO", "Seasoned specialist"],
  ["RAW", "Unprocessed sensor data"],
  ["RED", "Veloster N paint shade"],
  ["ROW", "Horizontal matrix vector"],
  ["SAW", "Cutoff blade"],
  ["SET", "Harden or cure"],
  ["SIT", "Rest in place"],
  ["SIX", "Three factorial"],
  ["SKI", "Alpine snow runner"],
  ["SUB", "Undersea vessel"],
  ["TAB", "Sheet-metal alignment ear"],
  ["TAG", "Equipment ID plate"],
  ["TAP", "Cut internal screw threads"],
  ["TAR", "Viscous pitch"],
  ["TEN", "Metric base"],
  ["TIE", "Tensile member"],
  ["TIP", "Outer blade radius"],
  ["TOE", "Wheel alignment angle"],
  ["TOP", "Upper dead center"],
  ["TOW", "Untwisted carbon fiber bundle"],
  ["TRY", "Attempt"],
  ["TUG", "Harbor boat"],
  ["TWO", "Smallest prime"],
  ["USE", "Put into service"],
  ["VAN", "Delivery vehicle"],
  ["VAT", "Fermentation tun"],
  ["VET", "Review a design"],
  ["VIA", "PCB plated through-hole"],
  ["WAX", "Lost-___ casting"],
  ["WAY", "Precision lathe guide rail"],
  ["WEB", "I-beam vertical plate"],
  ["WET", "Saturated"],
  ["WIN", "First-place finish"],
  ["WON", "Finished first"],
  ["YAW", "Vertical-axis rotation"],
  ["ANT", "Colony insect"],
  ["APE", "Primate"],
  ["APT", "Well-suited"],
  ["ASH", "Volcanic particulate"],
  ["ATE", "Consumed"],
  ["AXE", "Splitting wedge tool"],
  ["BAD", "Out of tolerance"],
  ["BAG", "Flour sack"],
  ["BAN", "Prohibit"],
  ["BAT", "Nocturnal flyer"],
  ["BED", "Lathe base casting"],
  ["BEE", "Pollinator"],
  ["BET", "Wager"],
  ["BID", "Contractor quote"],
  ["BIG", "___ Sur"],
  ["BIN", "Parts tray"],
  ["BOB", "Pendulum mass"],
  ["BOW", "Ship's front"],
  ["BOX", "Enclosure housing"],
  ["BUD", "Spring sprout"],
  ["BUG", "Code glitch"],
  ["BUN", "Brioche roll"],
  ["BUS", "Data communication line"],
  ["CAB", "Operator compartment"],
  ["CAN", "Sealed cylinder"],
  ["CAP", "Pipe end plug"],
  ["CAR", "Autocross entry"],
  ["COD", "Atlantic whitefish"],
  ["COT", "Camp bed"],
  ["CUP", "Eight fluid ounces"],
  ["CUT", "Lathe pass"],
  ["DAB", "Small amount"],
  ["DAD", "Family father"],
  ["DAM", "Reservoir barrier"],
  ["DAY", "24 hours"],
  ["DEN", "Study room"],
  ["DEW", "Condensation"],
  ["DIG", "Excavate"],
  ["DIM", "Low-lumen"],
  ["DIP", "Voltage sag"],
  ["DOT", "Scalar product symbol"],
  ["DRY", "Anhydrous"],
  ["DUE", "Scheduled"],
  ["DYE", "Penetrant inspection fluid"],
  ["EEL", "Moray fish"],
  ["EGG", "Brioche binder"],
  ["ELK", "Antlered wapiti"],
  ["ELM", "Shade tree"],
  ["EVE", "Night before"],
  ["EYE", "Storm center"],
  ["FAN", "Axial air mover"],
  ["FAR", "Distant"],
  ["FAT", "Lipid"],
  ["FED", "Supplied"],
  ["FEE", "Charge"],
  ["FEW", "Handful"],
  ["FIG", "Orchard fruit"],
  ["FIR", "Douglas timber"],
  ["FIT", "Clearance tolerance"],
  ["FIX", "Repair"],
  ["FLY", "___wheel"],
  ["FOG", "Low stratus cloud"],
  ["FOR", "Loop keyword"],
  ["FRY", "Sauté"],
  ["FUN", "Pastime"],
  ["GEL", "Colloidal network"],
  ["GEM", "Precious stone"],
  ["GET", "Retrieve"],
  ["GOT", "Obtained"],
  ["GUM", "Thickener"],
  ["GUN", "Heat ___"],
  ["GUY", "Tensioned cable"],
  ["GYM", "Weight room"],
  ["HAD", "Possessed"],
  ["HAM", "Radio operator"],
  ["HAT", "Hard ___"],
  ["HAY", "Baled feed"],
  ["HEM", "Folded metal edge"],
  ["HEX", "Bolt head shape"],
  ["HID", "Concealed"],
  ["HIP", "Roof ridge angle"],
  ["HOP", "Brewing cone"],
  ["HUE", "Wavelength color"],
  ["HUM", "60-Hz drone"],
  ["HUT", "Trail shelter"],
  ["ICY", "Rime-covered"],
  ["INK", "Plotter fluid"],
  ["INN", "Roadside lodge"],
  ["IRE", "Wrath"],
  ["IVY", "Climbing vine"],
  ["JAM", "Mechanical lockup"],
  ["JAW", "Caliper blade"],
  ["JOT", "Note quickly"],
  ["JUG", "Glass growler"],
  ["KEG", "Draft barrel"],
  ["KIT", "Assembly set"],
  ["LAB", "Testing room"],
  ["LAG", "Phase delay"],
  ["LAW", "Hooke's ___"],
  ["LAY", "Composite ply angle"],
  ["LED", "Diode lamp"],
  ["LEG", "Fillet weld size"],
  ["LET", "Allow"],
  ["LIP", "Shaft seal edge"],
  ["LIT", "Illuminated"],
  ["LOT", "Production batch"]
];

const WORD_MAP = new Map();
for (const [rawWord, clue] of RAW_DICTIONARY) {
  const w = rawWord.toUpperCase().trim();
  if (/^[A-Z]{3,5}$/.test(w) && !WORD_MAP.has(w)) {
    WORD_MAP.set(w, clue);
  }
}

const WORDS_BY_LEN = { 3: [], 4: [], 5: [] };
for (const [word] of WORD_MAP.entries()) {
  WORDS_BY_LEN[word.length].push(word);
}

const BASE_TEMPLATES = [
  [
    [0,0,0,1,1],
    [0,0,0,0,1],
    [0,0,0,0,0],
    [1,0,0,0,0],
    [1,1,0,0,0]
  ],
  [
    [0,0,0,0,1],
    [0,0,0,0,0],
    [0,0,0,0,0],
    [0,0,0,0,0],
    [1,0,0,0,0]
  ],
  [
    [1,0,0,0,0],
    [1,0,0,0,0],
    [0,0,0,0,0],
    [0,0,0,0,0],
    [0,0,0,0,1]
  ],
  [
    [0,0,0,0,0],
    [0,0,0,0,0],
    [0,0,0,0,0],
    [0,0,0,0,0],
    [0,0,0,0,0]
  ]
];

let currentMask = [];
let solutionGrid = [];
let userGrid = [];
let verifiedGrid = [];
let revealedGrid = [];
let cellNumbers = [];
let slots = [];
let activeCell = { r: 0, c: 0 };
let activeDir = "A";
let secondsElapsed = 0;
let timerInterval = null;
let isSolved = false;
let lastSig = "";

function shuffle(arr) {
  const a = arr.slice();
  for (let i = a.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [a[i], a[j]] = [a[j], a[i]];
  }
  return a;
}

function transformMask(mask, flipOption) {
  let m = mask.map(r => r.slice());
  if (flipOption & 1) m = m.map(r => r.slice().reverse());
  if (flipOption & 2) m = m.slice().reverse();
  return m;
}

function extractSlotsAndNumbers(mask) {
  const nums = Array.from({ length: 5 }, () => Array(5).fill(0));
  const extractedSlots = [];
  let nextNum = 1;

  for (let r = 0; r < 5; r++) {
    for (let c = 0; c < 5; c++) {
      if (mask[r][c] === 1) continue;
      const startsAcross = (c === 0 || mask[r][c - 1] === 1) && (c + 1 < 5 && mask[r][c + 1] === 0);
      const startsDown = (r === 0 || mask[r - 1][c] === 1) && (r + 1 < 5 && mask[r + 1][c] === 0);

      if (startsAcross || startsDown) nums[r][c] = nextNum++;

      if (startsAcross) {
        const cells = [];
        for (let cc = c; cc < 5 && mask[r][cc] === 0; cc++) cells.push([r, cc]);
        extractedSlots.push({ id: `${nums[r][c]}A`, num: nums[r][c], dir: "A", len: cells.length, cells });
      }
      if (startsDown) {
        const cells = [];
        for (let rr = r; rr < 5 && mask[rr][c] === 0; rr++) cells.push([rr, c]);
        extractedSlots.push({ id: `${nums[r][c]}D`, num: nums[r][c], dir: "D", len: cells.length, cells });
      }
    }
  }
  return { nums, extractedSlots };
}

function solveCrosswordFast(mask, maxNodes = 28000) {
  const { nums, extractedSlots } = extractSlotsAndNumbers(mask);
  const acrossSlots = extractedSlots.filter(s => s.dir === "A");
  const downSlots = extractedSlots.filter(s => s.dir === "D");

  const pools = {
    3: shuffle(WORDS_BY_LEN[3]),
    4: shuffle(WORDS_BY_LEN[4]),
    5: shuffle(WORDS_BY_LEN[5])
  };

  const prefixSets = { 3: new Set(), 4: new Set(), 5: new Set() };
  for (const len of [3, 4, 5]) {
    for (const w of pools[len]) {
      for (let k = 1; k <= len; k++) prefixSets[len].add(w.slice(0, k));
    }
  }

  const grid = Array.from({ length: 5 }, () => Array(5).fill(""));
  const usedWords = new Set();
  let nodes = 0;

  const orderedAcross = acrossSlots.slice().sort((a, b) => b.len - a.len);

  function checkDownConstraints() {
    for (const dSlot of downSlots) {
      let prefix = "";
      let full = true;
      for (let k = 0; k < dSlot.len; k++) {
        const [r, c] = dSlot.cells[k];
        const ch = grid[r][c];
        if (ch === "") {
          full = false;
          break;
        }
        prefix += ch;
      }
      if (prefix.length > 0 && !prefixSets[dSlot.len].has(prefix)) return false;
      if (full && usedWords.has(prefix)) return false;
    }
    return true;
  }

  function backtrackAcross(idx) {
    if (++nodes > maxNodes) return false;
    if (idx === orderedAcross.length) {
      const downSet = new Set();
      for (const dSlot of downSlots) {
        const w = dSlot.cells.map(([r, c]) => grid[r][c]).join("");
        if (!WORD_MAP.has(w) || usedWords.has(w) || downSet.has(w)) return false;
        downSet.add(w);
      }
      return true;
    }

    const slot = orderedAcross[idx];
    const candidates = pools[slot.len];

    for (let i = 0; i < candidates.length; i++) {
      const word = candidates[i];
      if (usedWords.has(word)) continue;

      for (let k = 0; k < slot.len; k++) {
        const [r, c] = slot.cells[k];
        grid[r][c] = word[k];
      }
      usedWords.add(word);

      if (checkDownConstraints() && backtrackAcross(idx + 1)) return true;

      usedWords.delete(word);
      for (let k = 0; k < slot.len; k++) {
        const [r, c] = slot.cells[k];
        grid[r][c] = "";
      }
    }
    return false;
  }

  if (!backtrackAcross(0)) return null;

  const finalSlots = extractedSlots.map(s => {
    const w = s.cells.map(([r, c]) => grid[r][c]).join("");
    return { ...s, word: w, clue: WORD_MAP.get(w) || "Crossword entry" };
  });

  return { nums, grid, finalSlots };
}

function generateNewPuzzle() {
  const selectVal = document.getElementById("templateSelect").value;
  let result = null;
  let chosenMask = null;

  for (let attempt = 0; attempt < 25; attempt++) {
    const baseIdx = selectVal === "random"
      ? Math.floor(Math.random() * BASE_TEMPLATES.length)
      : parseInt(selectVal, 10);

    const flipOption = Math.floor(Math.random() * 4);
    chosenMask = transformMask(BASE_TEMPLATES[baseIdx], flipOption);
    const candidate = solveCrosswordFast(chosenMask, 30000);
    if (candidate) {
      const sig = candidate.grid.map(r => r.join("")).join("|");
      if (sig !== lastSig) {
        result = candidate;
        lastSig = sig;
        break;
      }
    }
  }

  if (!result) {
    chosenMask = transformMask(BASE_TEMPLATES[0], Math.floor(Math.random() * 4));
    result = solveCrosswordFast(chosenMask, 80000);
  }

  currentMask = chosenMask;
  solutionGrid = result.grid;
  cellNumbers = result.nums;
  slots = result.finalSlots;

  userGrid = Array.from({ length: 5 }, () => Array(5).fill(""));
  verifiedGrid = Array.from({ length: 5 }, () => Array(5).fill(false));
  revealedGrid = Array.from({ length: 5 }, () => Array(5).fill(false));
  isSolved = false;

  document.getElementById("winModal").classList.remove("visible");
  document.getElementById("cluesModal").classList.remove("visible");

  const firstSlot = slots.find(s => s.dir === "A") || slots[0];
  activeCell = { r: firstSlot.cells[0][0], c: firstSlot.cells[0][1] };
  activeDir = firstSlot.dir;

  resetTimer();
  renderAll();
}

function resetTimer() {
  clearInterval(timerInterval);
  secondsElapsed = 0;
  updateTimerDisplay();
  timerInterval = setInterval(() => {
    if (!isSolved) {
      secondsElapsed++;
      updateTimerDisplay();
    }
  }, 1000);
}

function updateTimerDisplay() {
  const mins = Math.floor(secondsElapsed / 60);
  const secs = secondsElapsed % 60;
  document.getElementById("timer").textContent = `${mins}:${secs < 10 ? "0" : ""}${secs}`;
}

function getSlotAt(r, c, dir) {
  return slots.find(s => s.dir === dir && s.cells.some(([sr, sc]) => sr === r && sc === c));
}

function renderAll() {
  const currentSlot = getSlotAt(activeCell.r, activeCell.c, activeDir) ||
                      getSlotAt(activeCell.r, activeCell.c, activeDir === "A" ? "D" : "A");

  if (currentSlot && currentSlot.dir !== activeDir) activeDir = currentSlot.dir;

  const inWordSet = new Set(currentSlot ? currentSlot.cells.map(([r, c]) => `${r},${c}`) : []);
  const gridEl = document.getElementById("grid");
  gridEl.innerHTML = "";

  for (let r = 0; r < 5; r++) {
    for (let c = 0; c < 5; c++) {
      const cellEl = document.createElement("div");
      cellEl.className = "cell";

      if (currentMask[r][c] === 1) {
        cellEl.classList.add("black");
        gridEl.appendChild(cellEl);
        continue;
      }

      if (r === activeCell.r && c === activeCell.c) {
        cellEl.classList.add("active");
      } else if (inWordSet.has(`${r},${c}`)) {
        cellEl.classList.add("in-word");
      }

      if (verifiedGrid[r][c]) cellEl.classList.add("verified");
      if (revealedGrid[r][c]) cellEl.classList.add("revealed");

      if (cellNumbers[r][c] > 0) {
        const numSpan = document.createElement("span");
        numSpan.className = "num";
        numSpan.textContent = cellNumbers[r][c];
        cellEl.appendChild(numSpan);
      }

      const letterSpan = document.createElement("span");
      letterSpan.className = "letter";
      letterSpan.textContent = userGrid[r][c];
      cellEl.appendChild(letterSpan);

      cellEl.addEventListener("pointerdown", (e) => {
        e.preventDefault();
        if (activeCell.r === r && activeCell.c === c) {
          activeDir = activeDir === "A" ? "D" : "A";
        } else {
          activeCell = { r, c };
        }
        renderAll();
      });

      gridEl.appendChild(cellEl);
    }
  }

  if (currentSlot) {
    document.getElementById("bannerNum").textContent = currentSlot.id;
    document.getElementById("bannerText").textContent = currentSlot.clue;
  }
}

function advanceCursor(step = 1) {
  const slot = getSlotAt(activeCell.r, activeCell.c, activeDir);
  if (!slot) return;

  const idx = slot.cells.findIndex(([r, c]) => r === activeCell.r && c === activeCell.c);
  const nextIdx = idx + step;

  if (nextIdx >= 0 && nextIdx < slot.cells.length) {
    activeCell = { r: slot.cells[nextIdx][0], c: slot.cells[nextIdx][1] };
  } else if (step > 0) {
    const emptyInSlot = slot.cells.find(([r, c]) => userGrid[r][c] === "");
    if (emptyInSlot) {
      activeCell = { r: emptyInSlot[0], c: emptyInSlot[1] };
    } else {
      cycleClue(1);
    }
  }
}

function cycleClue(delta) {
  const curSlot = getSlotAt(activeCell.r, activeCell.c, activeDir);
  const curIdx = slots.findIndex(s => s.id === (curSlot && curSlot.id));
  const nextSlot = slots[(curIdx + delta + slots.length) % slots.length];
  activeDir = nextSlot.dir;
  const emptyCell = nextSlot.cells.find(([r, c]) => userGrid[r][c] === "");
  const target = emptyCell || nextSlot.cells[0];
  activeCell = { r: target[0], c: target[1] };
  renderAll();
}

function handleInputKey(key) {
  if (navigator.vibrate) navigator.vibrate(8);

  if (key === "FLIP") {
    activeDir = activeDir === "A" ? "D" : "A";
    renderAll();
    return;
  }

  if (key === "BACKSPACE") {
    if (isSolved) return;
    const { r, c } = activeCell;
    if (userGrid[r][c] !== "" && !verifiedGrid[r][c]) {
      userGrid[r][c] = "";
    } else {
      advanceCursor(-1);
      const nr = activeCell.r;
      const nc = activeCell.c;
      if (!verifiedGrid[nr][nc]) userGrid[nr][nc] = "";
    }
    renderAll();
    return;
  }

  if (/^[A-Z]$/.test(key)) {
    if (isSolved) return;
    const { r, c } = activeCell;
    if (!verifiedGrid[r][c]) {
      userGrid[r][c] = key;
    }
    advanceCursor(1);
    renderAll();
    checkVictory();
  }
}

function checkVictory() {
  for (let r = 0; r < 5; r++) {
    for (let c = 0; c < 5; c++) {
      if (currentMask[r][c] === 1) continue;
      if (userGrid[r][c] !== solutionGrid[r][c]) return;
    }
  }
  isSolved = true;
  clearInterval(timerInterval);
  const timeStr = document.getElementById("timer").textContent;
  document.getElementById("winStatsText").textContent =
    `You solved this ${slots.length}-word Mini in ${timeStr}!`;
  document.getElementById("winModal").classList.add("visible");
}

// On-Screen Touch Keyboard Listener
document.querySelectorAll(".key").forEach(btn => {
  btn.addEventListener("pointerdown", (e) => {
    e.preventDefault();
    btn.classList.add("pressed");
    handleInputKey(btn.dataset.key);
  });
  btn.addEventListener("pointerup", () => btn.classList.remove("pressed"));
  btn.addEventListener("pointercancel", () => btn.classList.remove("pressed"));
});

// Physical Keyboard Support (for desktop testing)
window.addEventListener("keydown", (e) => {
  if (e.metaKey || e.ctrlKey || e.altKey) return;
  if (/^[a-zA-Z]$/.test(e.key)) {
    e.preventDefault();
    handleInputKey(e.key.toUpperCase());
  } else if (e.key === "Backspace" || e.key === "Delete") {
    e.preventDefault();
    handleInputKey("BACKSPACE");
  } else if (e.key === " ") {
    e.preventDefault();
    handleInputKey("FLIP");
  } else if (e.key === "Tab") {
    e.preventDefault();
    cycleClue(e.shiftKey ? -1 : 1);
  }
});

// Clue Navigation Bar Listeners
document.getElementById("prevClueBtn").addEventListener("click", () => cycleClue(-1));
document.getElementById("nextClueBtn").addEventListener("click", () => cycleClue(1));
document.getElementById("clueBannerTap").addEventListener("click", () => handleInputKey("FLIP"));

// Top Toolbar Listeners
document.getElementById("newBtn").addEventListener("click", generateNewPuzzle);
document.getElementById("playAgainBtn").addEventListener("click", generateNewPuzzle);
document.getElementById("closeWinBtn").addEventListener("click", () => {
  document.getElementById("winModal").classList.remove("visible");
});
document.getElementById("templateSelect").addEventListener("change", generateNewPuzzle);

document.getElementById("checkBtn").addEventListener("click", () => {
  const gridCells = document.querySelectorAll(".grid .cell");
  let idx = 0;
  for (let r = 0; r < 5; r++) {
    for (let c = 0; c < 5; c++) {
      const cellEl = gridCells[idx++];
      if (currentMask[r][c] === 1 || userGrid[r][c] === "") continue;
      if (userGrid[r][c] === solutionGrid[r][c]) {
        verifiedGrid[r][c] = true;
        cellEl.classList.add("verified");
        cellEl.classList.remove("wrong");
      } else {
        cellEl.classList.add("wrong");
      }
    }
  }
});

document.getElementById("hintBtn").addEventListener("click", () => {
  const { r, c } = activeCell;
  if (currentMask[r][c] === 1) return;
  userGrid[r][c] = solutionGrid[r][c];
  verifiedGrid[r][c] = true;
  revealedGrid[r][c] = true;
  advanceCursor(1);
  renderAll();
  checkVictory();
});

// Full Clue List Drawer
document.getElementById("cluesBtn").addEventListener("click", () => {
  const container = document.getElementById("drawerContent");
  const across = slots.filter(s => s.dir === "A");
  const down = slots.filter(s => s.dir === "D");

  let html = "<h4>Across</h4>";
  for (const s of across) {
    html += `<div class="drawer-item" data-id="${s.id}"><b>${s.num}.</b> ${s.clue}</div>`;
  }
  html += "<h4>Down</h4>";
  for (const s of down) {
    html += `<div class="drawer-item" data-id="${s.id}"><b>${s.num}.</b> ${s.clue}</div>`;
  }
  container.innerHTML = html;

  container.querySelectorAll(".drawer-item").forEach(el => {
    el.addEventListener("click", () => {
      const slot = slots.find(s => s.id === el.dataset.id);
      if (slot) {
        activeDir = slot.dir;
        activeCell = { r: slot.cells[0][0], c: slot.cells[0][1] };
        document.getElementById("cluesModal").classList.remove("visible");
        renderAll();
      }
    });
  });

  document.getElementById("cluesModal").classList.add("visible");
});

document.getElementById("closeCluesBtn").addEventListener("click", () => {
  document.getElementById("cluesModal").classList.remove("visible");
});

document.getElementById("revealAllBtn").addEventListener("click", () => {
  for (let r = 0; r < 5; r++) {
    for (let c = 0; c < 5; c++) {
      if (currentMask[r][c] === 1) continue;
      if (userGrid[r][c] !== solutionGrid[r][c]) revealedGrid[r][c] = true;
      userGrid[r][c] = solutionGrid[r][c];
      verifiedGrid[r][c] = true;
    }
  }
  document.getElementById("cluesModal").classList.remove("visible");
  renderAll();
  checkVictory();
});

// Start first puzzle
generateNewPuzzle();
</script>
</body>
</html>
