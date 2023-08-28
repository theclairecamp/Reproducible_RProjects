# Reproducible_RProjects
Testing how to create reproducible R projects

Utilizing procedure found on: https://appsilon.com/renv-how-to-manage-dependencies-in-r/

Procedure for creating reproducible environment:
1. Activate renv environment
2. Install all packages for that environment
3. Take snapshot to initalize documentation of environment
4. Run analyses and re-take snapshot to update documentation
5. Transfer to git repo

Procedure for restoring R environment from renv()
1. git clone https://github.com/theclairecamp/<project>.git NewRenvProject
2. Open project that was downloaded
3. Then run - renv::restore() - to restore the R environment that was created for initial project
