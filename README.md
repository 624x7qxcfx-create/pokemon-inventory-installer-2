Repo to build the Pokémon Inventory Windows installer via GitHub Actions.

1) Create a new repository on GitHub.
2) Upload all files from this ZIP into the repo (in main branch).
3) In GitHub settings > Secrets, add TCG_PUBLIC_KEY and TCG_PRIVATE_KEY if desired for runtime (not needed for build).
4) Go to Actions tab, select 'Build Windows Installer' workflow and click 'Run workflow' (choose main branch).
5) When workflow completes, download the artifact named 'pokemon-windows-installer' from the run. This will be the installer .exe.

NOTE: You must approve GitHub Actions if prompted, and the first run may take ~10-20 minutes to complete. The Windows runner will build the backend exe and package the electron installer.
