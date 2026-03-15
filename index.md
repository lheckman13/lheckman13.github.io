<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Chicken Timeline Tracker</title>
  
  <script type="text/javascript" src="https://unpkg.com/vis-timeline@latest/standalone/umd/vis-timeline-graph2d.min.js"></script>
  <link href="https://unpkg.com/vis-timeline@latest/styles/vis-timeline-graph2d.min.css" rel="stylesheet" type="text/css" />

  <style>
    body { font-family: sans-serif; background-color: #f9f9f9; padding: 20px; }
    #visualization { border: 1px solid lightgray; background-color: white; border-radius: 8px; }
    .vis-item.got-chicken { background-color: #d1f7d1; border-color: #2e7d32; }
    .vis-item.dead-missing { background-color: #f7d1d1; border-color: #c62828; color: #7f0000; }
    h1 { color: #333; }
    .legend { margin-top: 10px; font-size: 0.9em; color: #666; }
  </style>
</head>
<body>

  <h1>🐔 Chicken Events Timeline</h1>
  <p>Drag to pan, scroll to zoom. Hover over events for notes.</p>
  
  <div id="visualization"></div>

  <div class="legend">
    <span style="color: #2e7d32;">●</span> Arrival (Got Chicken) | 
    <span style="color: #c62828;">●</span> Departure (Dead/Missing)
  </div>

  <script type="text/javascript">
    // 1. Define the Groups (Your Chickens)
    var groups = new vis.DataSet([
      { id: "Linda", content: "Linda" },
      { id: "Seamus", content: "Seamus" },
      { id: "Auroch", content: "Auroch" },
      { id: "Lucian", content: "Lucian" },
      { id: "Poirot", content: "Poirot" },
      { id: "Pigeon 1 (Boncho)", content: "Pigeon 1 (Boncho)" },
      { id: "Pigeon 2 (Overcoat)", content: "Pigeon 2 (Overcoat)" },
      { id: "Pigeon 3 (Young Guardian)", content: "Pigeon 3 (Young Guardian)" },
      { id: "Big Crow", content: "Big Crow" },
      { id: "Phoenix", content: "Phoenix" },
      { id: "Lavender", content: "Lavender" },
      { id: "Coward", content: "Coward" }
    ]);

    // 2. Define the Items (Your Events)
    var items = new vis.DataSet([
      { id: 0, group: "Linda", content: "got chicken", start: "2025-06-30", className: "got-chicken" },
      { id: 1, group: "Seamus", content: "got chicken", start: "2025-06-30", className: "got-chicken" },
      { id: 2, group: "Seamus", content: "missing", start: "2025-08-15", className: "dead-missing" },
      { id: 3, group: "Auroch", content: "got chicken", start: "2025-07-15", className: "got-chicken" },
      { id: 4, group: "Auroch", content: "missing", start: "2025-08-15", className: "dead-missing" },
      { id: 5, group: "Auroch", content: "dead", start: "2026-03-07", className: "dead-missing", title: "Sour crop - possibly murdered by us" },
      { id: 6, group: "Lucian", content: "dead", start: "2025-08-15", className: "dead-missing", title: "Hawk ate her" },
      { id: 7, group: "Lucian", content: "got chicken", start: "2025-07-15", className: "got-chicken" },
      { id: 8, group: "Poirot", content: "dead", start: "2025-08-06", className: "dead-missing" },
      { id: 9, group: "Poirot", content: "got chicken", start: "2025-07-15", className: "got-chicken" },
      { id: 10, group: "Pigeon 1 (Boncho)", content: "got chicken", start: "2025-08-15", className: "got-chicken" },
      { id: 11, group: "Pigeon 1 (Boncho)", content: "dead", start: "2026-02-21", className: "dead-missing", title: "est. date - unknown predator got her" },
      { id: 12, group: "Pigeon 2 (Overcoat)", content: "got chicken", start: "2025-08-15", className: "got-chicken" },
      { id: 13, group: "Pigeon 2 (Overcoat)", content: "dead", start: "2025-09-10", className: "dead-missing", title: "est. date" },
      { id: 14, group: "Pigeon 3 (Young Guardian)", content: "got chicken", start: "2025-08-15", className: "got-chicken" },
      { id: 15, group: "Big Crow", content: "got chicken", start: "2025-09-28", className: "got-chicken" },
      { id: 16, group: "Phoenix", content: "got chicken", start: "2025-09-28", className: "got-chicken" },
      { id: 17, group: "Lavender", content: "got chicken", start: "2025-09-28", className: "got-chicken" },
      { id: 18, group: "Coward", content: "got chicken", start: "2025-09-28", className: "got-chicken" }
    ]);

    // 3. Configuration options
    var options = {
      stack: true, // Prevent events from overlapping
      horizontalScroll: true,
      zoomKey: 'ctrlKey', // Zoom only if ctrl is held, otherwise scroll to pan
      orientation: 'top',
      maxHeight: '600px',
      start: '2025-06-01',
      end: '2026-04-01'
    };

    // 4. Create the Timeline
    var container = document.getElementById('visualization');
    var timeline = new vis.Timeline(container, items, groups, options);
  </script>
</body>
</html>
