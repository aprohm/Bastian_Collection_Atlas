# Bastian Collection Atlas

An interactive atlas of Adolf Bastian's acquisitions for the Königliches Museum für Völkerkunde, Berlin (founded 1873, opened 1886). The objects and letters can be explored in seven view modes: Museum, Cabinet, Map, Globe, Web, Data and Atlas.

Concept, research, design and construction: [Alan Prohm](https://alanprohm.com/), coded with Claude.
Collection data: Deutsche Digitale Bibliothek (DDB) / Ethnologisches Museum, Staatliche Museen zu Berlin.

## What is in this folder

| File | Purpose |
|---|---|
| `index.html` | The whole site in one self-contained file (about 22 MB). Data, images, fonts and the map, globe and graph libraries are all embedded. |
| `.nojekyll` | Tells GitHub Pages to serve the file as it is, without running it through Jekyll. |
| `README.md` | This page. |

The site runs from this single file. It needs no build step and no server code. Only two things use the internet when it is available: close-up satellite imagery on the Map, and object thumbnails from the museum's image server.

## Publish with GitHub Pages

1. On github.com, create a new repository, for example `bastian-collection-atlas`, and make it public.
2. On the repository page, choose **Add file › Upload files** and drag in the contents of this folder: `index.html`, `README.md` and `.nojekyll`. Then commit.
   - `.nojekyll` is a hidden file. If your file browser hides it, you can skip it; the site will still work.
3. Go to **Settings › Pages**. Under *Build and deployment*, set **Source** to *Deploy from a branch*, choose the branch `main` and the folder `/ (root)`, and click **Save**.
4. After a minute or two, the site is live at `https://<your-username>.github.io/bastian-collection-atlas/`.

To update the site later, upload a new `index.html` over the old one and commit. Pages republishes automatically.

### From the command line instead

```bash
cd bastian-collection-atlas
git init
git add .
git commit -m "Bastian Collection Atlas"
git branch -M main
git remote add origin https://github.com/<your-username>/bastian-collection-atlas.git
git push -u origin main
```

Then enable Pages as in step 3 above.

## Browser notes

- Works in current Chrome, Firefox, Safari and Edge.
- The Globe and Web views use 3D graphics (WebGL). If a browser has 3D graphics switched off, both views fall back to a flat 2D version, and a note explains how to re-enable 3D. Add `#flat` to the address to try the flat versions.

## Credits and rights

- Atlas plates: Adolf Bastian, *Die wechselnden Phasen im geschichtlichen Sehkreis*, Berlin: Dietrich Reimer (Ernst Vohsen), 1900, public domain; scans by Alan Prohm.
- Museum floor plans: *Führer durch das Museum für Völkerkunde*, 15th ed., 1911.
- Historical photographs and drawings are credited individually in the site.
- Object records and images remain under the licences stated by the Staatliche Museen zu Berlin and the Deutsche Digitale Bibliothek (shown with each record).

No licence has been chosen for the site's own code and design yet. Until one is added, all rights are reserved by the author.
