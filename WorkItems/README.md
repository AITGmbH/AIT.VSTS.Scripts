# AIT.Scripts.WorkItems

Contains PowerShell Scripts for TFS-WorkItem manipulation.

## Create-Backlog-Item-And-Tasks-For-Team-Members.ps1

Automatically creates a single Product Backlog Item (PBI) for a team and a workitem for every member within the team.

SPACES IN ARGUMENTS MUST BE ENCLOSED BY SINGLE QUOTES

Example: Create the items with the given title for the given server.
  .\Create-Team-Work-Items -Url "https://example.visualstudio.com/DefaultCollection" -ProjectName "MyProject" -Team "ExampleTeam" -Title "My New Work Item Title" -WorkItemType "Requirement"

Known Bugs:
When your DisplayName's are not unique one of the duplicates with get all workitems. See 
- http://stackoverflow.com/questions/16295066/not-getting-field-assigned-to-and-last-update-date-of-workitem-from-the-work
- https://stackoverflow.com/questions/30641279/how-to-set-assigned-to-in-tfs-work-item-through-code#
