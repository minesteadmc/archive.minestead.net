# archive.minestead.net

A weekly timelapse of the Minestead world map. Drag the timeline at the bottom, or press play, to see how the world has changed.

This is a static site served by GitHub Pages. `index.html` is the viewer, and `store/` holds the map tiles.

- Each snapshot is a folder in `store/`. The first holds the full map, and each later one holds only the tiles that changed since the snapshot before it.
- `store/index.json` lists which snapshots have a copy of each changed tile. For any date, the viewer uses the newest copy on or before that date.
- Map tiles are rendered by [Dynmap](https://github.com/webbukkit/dynmap).

To preview locally, run `python3 -m http.server 8765` in this folder and open http://localhost:8765.
