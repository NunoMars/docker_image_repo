# Docker Image build and push to GitHub Registry

Github action qui permet de build et push une image docker sur le GItHub Container Registry

Pour utiliser l'action:

```bash
    - name: Docker Image build and push to GitHub Container Registry
    uses: NunoMars/docker_image_repo@v0.2
    with:
      file: Dockerfile
      image: 'your-image-name'
      tag: ${{ github.ref_slug }}
      context: '.'
      github-token: ${{ secrets.GITHUB_TOKEN}}
```
