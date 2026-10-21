# Panel de cobro EDC

Página estática (GitHub Pages). Los datos van **cifrados con AES-256-GCM** y se descifran en el navegador
con la contraseña del equipo. No hay backend ni base de datos: el repositorio solo contiene el HTML y el blob cifrado.

## Cambiar la contraseña

```bash
EDC_PW='nueva-contraseña' python3 build_publish.py
```

y volver a publicar (`git commit` + `git push`).

## Aviso

La contraseña protege el contenido, no el enlace. Si el enlace se filtra, la única barrera es la contraseña:
cuanto más larga, mejor. Rota la clave si sale del equipo.
