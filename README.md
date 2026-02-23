# Wikidata REST API Examples
This is a collection of Wikidata REST API endpoint examples in Bruno's .bru file format. You can use these examples with Bruno or another API client to try out Wikibase REST API requests.

More information about the Wikibase REST API can be found in the [documentation](https://doc.wikimedia.org/Wikibase/master/js/rest-api/#/).

## Description
In the `endpoint-collection` directory you will find folders that contain the individual requests. These folders are sorted by the data that the requests call and include items, labels, descriptions, aliases, properties, sitelinks and statements. `endpoint-collection` also contains a bruno.json and a collection.bru file. Another folder within this directory named `environments` contains .bru files for each of the collection's environments. In these files the environment variables are saved. The variables store dynamic values that can be reused across multiple requests. They are used in the endpoints with double curly braces: `{{base-url}}/entities/items/{{item-id}}`.

The examples in this collection can be used as they are with Bruno. They can also be used with other API clients after converting them to that software's file format.

## Usage with Bruno
### First steps
1. Download [Bruno](https://www.usebruno.com/downloads).
2. Clone this repository: `git clone https://github.com/wmde/wikidata-rest-api-examples`
3. In Bruno, click "Import collection" and select the directory containing the .bru files.
4. In the top right corner choose an environment to work in. This can be adjusted at any point.
> When trying out the REST API, use the Wikidata environment for fetching. You can also use this environment to edit the sandbox item, which is defined in a variable of the same name. When creating and deleting items, use the Beta Wikidata environment.
5. Select individual requests and execute the request by clicking the arrow or pressing Ctrl + Enter.

### Making changes: Environment Variables
1. Navigate to the collection overview and click collection environments.
2. Create new environments by selecting the + symbol.
3. Edit existing environment variables on the right by adding or editing the Name and Value.
4. Click save.