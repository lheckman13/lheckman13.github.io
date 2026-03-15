<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Chicken Timeline Tracker</title>
  
  <script type="text/javascript" src="https://unpkg.com/vis-timeline@latest/standalone/umd/vis-timeline-graph2d.min.js"></script>
  <link href="https://unpkg.com/vis-timeline@latest/styles/vis-timeline-graph2d.min.css" rel="stylesheet" type="text/css" />

  <style>
    /* Make the page use the full screen width */
    body { 
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; 
      background-color: #f9f9f9; 
      margin: 0; 
      padding: 20px; 
    }
    
    h1 { margin-top: 0; color: #333; }

    /* The container now fills the width */
    #visualization { 
      width: 100%; 
      border: 1px solid #ddd; 
      background-color: white; 
      border-radius: 8px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.05);
    }

    /* Visual styles for your event types */
    .vis-item.got-chicken { 
      background-color: #d1f7d1 !important; 
      border-color: #2e7d32 !important; 
      font-weight: bold;
    }
    .vis-item.dead-missing { 
      background-color: #f7d1d1 !important; 
      border-color: #c62828 !important; 
      color: #7f0000 !important; 
    }
    
    /* Make the chicken names on the left a bit wider/bolder */
    .vis-label { font-weight: 600; font-size: 14px; }

    .legend { margin-top: 15px; font-size: 0.9em; color: #555; }
  </style>
</head>
<body>

  <h1>🐔 Chicken Events Timeline</h1>
  
  <div id="visualization"></div>

  <div class="legend">
    <strong>Legend:</strong> 
    <span style="color: #2e7d32;">●</span> Arrival | 
    <span style="color: #c62828;">●</span> Departure (Dead/Missing) | 
    <em>Scroll to Zoom • Drag to Pan • Ctrl+Scroll to Zoom faster</em>
  </div>

  <script type="text/javascript">
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

    var items = new vis.DataSet([
      { id: 0, group: "Linda", content: "got chicken", start: "2025-06-30", className: "got-chicken" },
      { id: 1, group: "Seamus", content: "got chicken", start: "2025-06-30", className: "got-chicken" },
      { id: 2, group: "Seamus", content: "missing", start: "2025-08-15", className: "dead-missing" },
      { id: 3, group: "Auroch", content: "got chicken", start: "2025-07-15", className: "got-chicken" },
      { id: 4, group: "Auroch", content: "missing", start: "2025-08-15", className: "dead-missing" },
      { id: 5, group: "Auroch", content: "dead", start: "2026-03-07", className: "dead-missing", title: "Sour crop" },
      { id: 6, group: "Lucian", content: "dead", start: "2025-08-15", className: "dead-missing", title: "Hawk ate her" },
      { id: 7, group: "Lucian", content: "got chicken", start: "2025-07-15", className: "got-chicken" },
      { id: 8, group: "Poirot", content: "dead", start: "2025-08-06", className: "dead-missing" },
      { id: 9, group: "Poirot", content: "got chicken", start: "2025-07-15", className: "got-chicken" },
      { id: 10, group: "Pigeon 1 (Boncho)", content: "got chicken", start: "2025-08-15", className: "got-chicken" },
      { id: 11, group: "Pigeon 1 (Boncho)", content: "dead", start: "2026-02-21", className: "dead-missing" },
      { id: 12, group: "Pigeon 2 (Overcoat)", content: "got chicken", start: "2025-08-15", className: "got-chicken" },
      { id: 13, group: "Pigeon 2 (Overcoat)", content: "dead", start: "2025-09-10", className: "dead-missing" },
      { id: 14, group: "Pigeon 3 (Young Guardian)", content: "got chicken", start: "2025-08-15", className: "got-chicken" },
      { id: 15, group: "Big Crow", content: "got chicken", start: "2025-09-28", className: "got-chicken" },
      { id: 16, group: "Phoenix", content: "got chicken", start: "2025-09-28", className: "got-chicken" },
      { id: 17, group: "Lavender", content: "got chicken", start: "2025-09-28", className: "got-chicken" },
      { id: 18, group: "Coward", content: "got chicken", start: "2025-09-28", className: "got-chicken" }
    ]);

    var options = {
      width: '100%',
      height: 'auto',
      minHeight: '400px',
      stack: true,
      showCurrentTime: true,
      // Setting a specific start/end date range to make it look "wider" on load
      start: '2025-06-15',
      end: '2025-10-15', 
      zoomMin: 1000 * 60 * 60 * 24 * 7, // Min zoom is 1 week
      zoomMax: 1000 * 60 * 60 * 24 * 365 * 2, // Max zoom is 2 years
      margin: {
        item: 20, // Vertical space between items
        axis: 40  // Space between items and the bottom axis
      },
      orientation: 'top'
    };

    var container = document.getElementById('visualization');
    var timeline = new vis.Timeline(container, items, groups, options);
  </script>
</body>
</html>
