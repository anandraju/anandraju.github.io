#GitHub Issues

## PowerShell Snippets

### Get List of Issues

The following snippet gets a list of issues from a GitHub repository.

```
# Generate the authorization header
$bytes = [System.Text.Encoding]::UTF8.GetBytes("username:password")
$encoded = [System.Convert]::ToBase64String($bytes);
$auth1 = "Basic $encoded"

# Set url and send REST request
# - pages of 30 results at a time are returned use query string ?page=n to retrieve next page.
$url = "https://api.github.com/repos/anandraju/shuts/issues" # 
Invoke-RestMethod -Uri $url -Headers @{"AUTHORIZATION"=$auth} -Method GET

```
