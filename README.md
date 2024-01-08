# Docker Image build and push to GitHub Registry

Github action qui permet de build et push une image docker sur le GItHub Container Registry

Pour utiliser l'action:

```bash
    - name: Docker Image build and push to GitHub Container Registry
    uses: NunoMars/docker_image_repo@v0.2
    with:
      image_name: 'your-image-name'
      tag: ${{ github.ref_slug }}
      context: '.'
```
