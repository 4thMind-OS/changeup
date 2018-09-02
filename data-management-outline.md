# Example of an enterprise level UI data management architecture
- The Views know about ViewModels
- ViewModels know about ModelResources
- ModelResources know about
  - Service integrations
  - DTO models (the ones that are relevant to the models they own)
  - Models (the client side representation that DTOs get turned into...maybe decorated a bit with display string specific formatters/helpers)
  

## App-Page_view  
  
View for an app that allows users to see information about their coding team, the team’s apps, servers, and the current user’s own apps and servers  
  
## App-Page_view[Component]  
  
### [MODEL] App-Page_viewModel  
  
* CurrentUserModelResource  
    * DATA  
        * User_Model  
        * User-Apps_Resource  
            * App_Model  
        * User-Servers_Resource  
            * Server_Model  
        * PermissionsResource  
            * Permission_Model  
        * PetsResource  
            * Pet_Model  
                * Pet_dto  
        * Favorite Color  
        * UserCustomPreferences  
    * ACTIONS  
        * UpdatePermissions(...)  
        * DeletePermissions(...)  
        * HugPets(...)  
* UsersModelResource  
    * (a query that lets you get info about a group of people...in this case a team)  
    * Users_Model  
* FiltersModelResiource  
* AppsResource  
    * AppsModel  
        * AppModel  
* ServersResource  
  
### SubComponents  
  
* Filters  
    * Various Form Components  
* Metric Summaries  
    * SummaryTiles  
* CustomTableComponent  
    * Table Toolbar  
    * Talble  
