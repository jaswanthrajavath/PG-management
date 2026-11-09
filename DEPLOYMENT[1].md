# Vercel deployment checklist

1. Commit the contents of this folder to the root of your GitHub `main` branch.
2. In Vercel, choose Framework Preset `Other`.
3. Set Root Directory to `./`.
4. Leave Build Command and Install Command empty.
5. Set Output Directory to `.`.
6. Deploy and open the production URL.
7. In Chrome DevTools → Application → Service Workers, confirm `sw.js` is activated.
8. Open the app once while online, then test offline navigation.
9. In Settings → Export, download a JSON backup and verify it is non-empty.
