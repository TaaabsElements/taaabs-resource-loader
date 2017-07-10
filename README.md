# taaabs-resource-loader

`<taaabs-resource-loader>` loads and stores some kTBS resources.
The main goal of this component is to make sure the resource loading requests won't saturate the kTBS server.

## Example

If you have several component that load kTBS resource on the same page, proceed as follows:

    <taaabs-resource-loader resources={{shared_resources}} is-loading={{shared_loading_resources_status}} loading-list={{shared_loading_resources}}>
      <taaabs-base-graph base-url="[[baseUrl]]" taaabs-central-loading>
      </taaabs-base-graph>
    </taaabs-resource-loader>

    <taaabs-resource-loader resources={{shared_resources}} is-loading={{shared_loading_resources_status}} loading-list={{shared_loading_resources}}>
      <taaabs-trace-details-container trace-url="[[traceUrl]]" taaabs-central-loading>
      </taaabs-trace-details-container>
    </taaabs-resource-loader>

## TODO
