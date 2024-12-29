# Docker Image build and push to GitHub Registry

Github action qui permet de build et push une image docker sur le GItHub Container Registry

Pour utiliser l'action:

```bash
    - name: Docker Image build and push to GitHub Container Registry
    uses: NunoMars/docker_image_repo@v3.0
    with:
      username: 'your username'
      image-name: 'your-image-name'
      context: '.'
      password: ${{ secrets.GITHUB_TOKEN}}
```
