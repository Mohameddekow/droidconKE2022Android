## Contributing

- Find an issue in the [project board](https://github.com/orgs/droidconKE/projects/1/views/1) and assign it to yourself. You can also create an issue if it doesn't exist.
- Create a branch against main
- Create a PR to main. PullRequests must pass the following checks;
    * Must be approved by a code owner
    * Must pass all CI Checks
    * Must include updated tests
    * Must have every conversation resolved before merging
- We encourage you to use [git rebase](https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase#:~:text=What%20is%20git%20rebase%3F,of%20a%20feature%20branching%20workflow.) for a linear history


## Naming conventions
- All Compose navigation Destination components must be suffixed with `Screen` ie. `HomeScreen`
- All components inside a screen must be suffixed with suffixed with the word `Component` ie. `SponsorsComponent`
- All ViewModels must be suffixed with the word `ViewModel` ie. `HomeViewModel`
- All useCases must be prefixed with a get or set depending on functionality and suffixed with Usecase ie. `GetSponsorsUsecase`
- All repositories must be suffixed with Repository. ie. `SponsorsRepository`
- All repository implementations must be suffixed with `DataRepository` ie. `SponsorsDataRepository`
- All public functions in the ViewModel must be prefixed with `on` and suffixed with `action` ie. `onSignInAction()`
- All models should suffix the layer then model. ie. `SponsorsDataModel` or `SponsorsDomainModel` or `SponsorsPresentationModel`
- All mappers should follow the pattern `model-layerFrom-layerTo-mapper` ie. `SponsorDataToDomainMapper`


## Coding Style
### DO
- ViewModel and view will fall under the feature's Ui package
- All Ui components will be under feature's components package
- Include tests if you are making changes to the following;
    - ViewModel
    - Repository
    - Usecase
    - Mappers
- Format your changed files `COMMAND+OPTION+L` for mac users or `CTRL+ALT+L`
- Include a preview for all UI components.

### DON'T
- Don't include the word `impl` in a repository implementation name. Use `DataRepository` instead.
