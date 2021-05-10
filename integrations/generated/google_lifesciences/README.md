# @datafire/google_lifesciences

Client library for Cloud Life Sciences API

## Installation and Usage
```bash
npm install --save @datafire/google_lifesciences
```
```js
let google_lifesciences = require('@datafire/google_lifesciences').create({
  access_token: "",
  refresh_token: "",
  client_id: "",
  client_secret: "",
  redirect_uri: ""
});

.then(data => {
  console.log(data);
});
```

## Description

Cloud Life Sciences is a suite of services and tools for managing, processing, and transforming life sciences data.

## Actions

### oauthCallback
Exchange the code passed to your redirect URI for an access_token


```js
google_lifesciences.oauthCallback({
  "code": ""
}, context)
```

#### Input
* input `object`
  * code **required** `string`

#### Output
* output `object`
  * access_token `string`
  * refresh_token `string`
  * token_type `string`
  * scope `string`
  * expiration `string`

### oauthRefresh
Exchange a refresh_token for an access_token


```js
google_lifesciences.oauthRefresh(null, context)
```

#### Input
*This action has no parameters*

#### Output
* output `object`
  * access_token `string`
  * refresh_token `string`
  * token_type `string`
  * scope `string`
  * expiration `string`

### lifesciences.projects.locations.operations.get
Gets the latest state of a long-running operation. Clients can use this method to poll the operation result at intervals as recommended by the API service. Authorization requires the following [Google IAM](https://cloud.google.com/iam) permission: * `lifesciences.operations.get`


```js
google_lifesciences.lifesciences.projects.locations.operations.get({
  "name": ""
}, context)
```

#### Input
* input `object`
  * name **required** `string`: The name of the operation resource.
  * $.xgafv `string` (values: 1, 2): V1 error format.
  * access_token `string`: OAuth access token.
  * alt `string` (values: json, media, proto): Data format for response.
  * callback `string`: JSONP
  * fields `string`: Selector specifying which fields to include in a partial response.
  * key `string`: API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
  * oauth_token `string`: OAuth 2.0 token for the current user.
  * prettyPrint `boolean`: Returns response with indentations and line breaks.
  * quotaUser `string`: Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
  * upload_protocol `string`: Upload protocol for media (e.g. "raw", "multipart").
  * uploadType `string`: Legacy upload protocol for media (e.g. "media", "multipart").

#### Output
* output [Operation](#operation)

### lifesciences.projects.locations.list
Lists information about the supported locations for this service.


```js
google_lifesciences.lifesciences.projects.locations.list({
  "name": ""
}, context)
```

#### Input
* input `object`
  * name **required** `string`: The resource that owns the locations collection, if applicable.
  * filter `string`: The standard list filter.
  * pageSize `integer`: The standard list page size.
  * pageToken `string`: The standard list page token.
  * $.xgafv `string` (values: 1, 2): V1 error format.
  * access_token `string`: OAuth access token.
  * alt `string` (values: json, media, proto): Data format for response.
  * callback `string`: JSONP
  * fields `string`: Selector specifying which fields to include in a partial response.
  * key `string`: API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
  * oauth_token `string`: OAuth 2.0 token for the current user.
  * prettyPrint `boolean`: Returns response with indentations and line breaks.
  * quotaUser `string`: Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
  * upload_protocol `string`: Upload protocol for media (e.g. "raw", "multipart").
  * uploadType `string`: Legacy upload protocol for media (e.g. "media", "multipart").

#### Output
* output [ListLocationsResponse](#listlocationsresponse)

### lifesciences.projects.locations.operations.list
Lists operations that match the specified filter in the request. Authorization requires the following [Google IAM](https://cloud.google.com/iam) permission: * `lifesciences.operations.list`


```js
google_lifesciences.lifesciences.projects.locations.operations.list({
  "name": ""
}, context)
```

#### Input
* input `object`
  * name **required** `string`: The name of the operation's parent resource.
  * filter `string`: A string for filtering Operations. The following filter fields are supported: * createTime: The time this job was created * events: The set of event (names) that have occurred while running the pipeline. The : operator can be used to determine if a particular event has occurred. * error: If the pipeline is running, this value is NULL. Once the pipeline finishes, the value is the standard Google error code. * labels.key or labels."key with space" where key is a label key. * done: If the pipeline is running, this value is false. Once the pipeline finishes, the value is true.
  * pageSize `integer`: The maximum number of results to return. The maximum value is 256.
  * pageToken `string`: The standard list page token.
  * $.xgafv `string` (values: 1, 2): V1 error format.
  * access_token `string`: OAuth access token.
  * alt `string` (values: json, media, proto): Data format for response.
  * callback `string`: JSONP
  * fields `string`: Selector specifying which fields to include in a partial response.
  * key `string`: API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
  * oauth_token `string`: OAuth 2.0 token for the current user.
  * prettyPrint `boolean`: Returns response with indentations and line breaks.
  * quotaUser `string`: Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
  * upload_protocol `string`: Upload protocol for media (e.g. "raw", "multipart").
  * uploadType `string`: Legacy upload protocol for media (e.g. "media", "multipart").

#### Output
* output [ListOperationsResponse](#listoperationsresponse)

### lifesciences.projects.locations.operations.cancel
Starts asynchronous cancellation on a long-running operation. The server makes a best effort to cancel the operation, but success is not guaranteed. Clients may use Operations.GetOperation or Operations.ListOperations to check whether the cancellation succeeded or the operation completed despite cancellation. Authorization requires the following [Google IAM](https://cloud.google.com/iam) permission: * `lifesciences.operations.cancel`


```js
google_lifesciences.lifesciences.projects.locations.operations.cancel({
  "name": ""
}, context)
```

#### Input
* input `object`
  * name **required** `string`: The name of the operation resource to be cancelled.
  * body [CancelOperationRequest](#canceloperationrequest)
  * $.xgafv `string` (values: 1, 2): V1 error format.
  * access_token `string`: OAuth access token.
  * alt `string` (values: json, media, proto): Data format for response.
  * callback `string`: JSONP
  * fields `string`: Selector specifying which fields to include in a partial response.
  * key `string`: API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
  * oauth_token `string`: OAuth 2.0 token for the current user.
  * prettyPrint `boolean`: Returns response with indentations and line breaks.
  * quotaUser `string`: Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
  * upload_protocol `string`: Upload protocol for media (e.g. "raw", "multipart").
  * uploadType `string`: Legacy upload protocol for media (e.g. "media", "multipart").

#### Output
* output [Empty](#empty)

### lifesciences.projects.locations.pipelines.run
Runs a pipeline. The returned Operation's metadata field will contain a google.cloud.lifesciences.v2beta.Metadata object describing the status of the pipeline execution. The response field will contain a google.cloud.lifesciences.v2beta.RunPipelineResponse object if the pipeline completes successfully. **Note:** Before you can use this method, the *Life Sciences Service Agent* must have access to your project. This is done automatically when the Cloud Life Sciences API is first enabled, but if you delete this permission you must disable and re-enable the API to grant the Life Sciences Service Agent the required permissions. Authorization requires the following [Google IAM](https://cloud.google.com/iam/) permission: * `lifesciences.workflows.run`


```js
google_lifesciences.lifesciences.projects.locations.pipelines.run({
  "parent": ""
}, context)
```

#### Input
* input `object`
  * parent **required** `string`: The project and location that this request should be executed against.
  * body [RunPipelineRequest](#runpipelinerequest)
  * $.xgafv `string` (values: 1, 2): V1 error format.
  * access_token `string`: OAuth access token.
  * alt `string` (values: json, media, proto): Data format for response.
  * callback `string`: JSONP
  * fields `string`: Selector specifying which fields to include in a partial response.
  * key `string`: API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
  * oauth_token `string`: OAuth 2.0 token for the current user.
  * prettyPrint `boolean`: Returns response with indentations and line breaks.
  * quotaUser `string`: Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
  * upload_protocol `string`: Upload protocol for media (e.g. "raw", "multipart").
  * uploadType `string`: Legacy upload protocol for media (e.g. "media", "multipart").

#### Output
* output [Operation](#operation)



## Definitions

### Accelerator
* Accelerator `object`: Carries information about an accelerator that can be attached to a VM.
  * count `string`: How many accelerators of this type to attach.
  * type `string`: The accelerator type string (for example, "nvidia-tesla-k80"). Only NVIDIA GPU accelerators are currently supported. If an NVIDIA GPU is attached, the required runtime libraries will be made available to all containers under `/usr/local/nvidia`. The driver version to install must be specified using the NVIDIA driver version parameter on the virtual machine specification. Note that attaching a GPU increases the worker VM startup time by a few minutes.

### Action
* Action `object`: Specifies a single action that runs a Docker container.
  * alwaysRun `boolean`: By default, after an action fails, no further actions are run. This flag indicates that this action must be run even if the pipeline has already failed. This is useful for actions that copy output files off of the VM or for debugging. Note that no actions will be run if image prefetching fails.
  * commands `array`: If specified, overrides the `CMD` specified in the container. If the container also has an `ENTRYPOINT` the values are used as entrypoint arguments. Otherwise, they are used as a command and arguments to run inside the container.
    * items `string`
  * containerName `string`: An optional name for the container. The container hostname will be set to this name, making it useful for inter-container communication. The name must contain only upper and lowercase alphanumeric characters and hyphens and cannot start with a hyphen.
  * credentials [Secret](#secret)
  * disableImagePrefetch `boolean`: All container images are typically downloaded before any actions are executed. This helps prevent typos in URIs or issues like lack of disk space from wasting large amounts of compute resources. If set, this flag prevents the worker from downloading the image until just before the action is executed.
  * disableStandardErrorCapture `boolean`: A small portion of the container's standard error stream is typically captured and returned inside the `ContainerStoppedEvent`. Setting this flag disables this functionality.
  * enableFuse `boolean`: Enable access to the FUSE device for this action. Filesystems can then be mounted into disks shared with other actions. The other actions do not need the `enable_fuse` flag to access the mounted filesystem. This has the effect of causing the container to be executed with `CAP_SYS_ADMIN` and exposes `/dev/fuse` to the container, so use it only for containers you trust.
  * entrypoint `string`: If specified, overrides the `ENTRYPOINT` specified in the container.
  * environment `object`: The environment to pass into the container. This environment is merged with values specified in the google.cloud.lifesciences.v2beta.Pipeline message, overwriting any duplicate values. In addition to the values passed here, a few other values are automatically injected into the environment. These cannot be hidden or overwritten. `GOOGLE_PIPELINE_FAILED` will be set to "1" if the pipeline failed because an action has exited with a non-zero status (and did not have the `IGNORE_EXIT_STATUS` flag set). This can be used to determine if additional debug or logging actions should execute. `GOOGLE_LAST_EXIT_STATUS` will be set to the exit status of the last non-background action that executed. This can be used by workflow engine authors to determine whether an individual action has succeeded or failed.
  * ignoreExitStatus `boolean`: Normally, a non-zero exit status causes the pipeline to fail. This flag allows execution of other actions to continue instead.
  * imageUri `string`: Required. The URI to pull the container image from. Note that all images referenced by actions in the pipeline are pulled before the first action runs. If multiple actions reference the same image, it is only pulled once, ensuring that the same image is used for all actions in a single pipeline. The image URI can be either a complete host and image specification (e.g., quay.io/biocontainers/samtools), a library and image name (e.g., google/cloud-sdk) or a bare image name ('bash') to pull from the default library. No schema is required in any of these cases. If the specified image is not public, the service account specified for the Virtual Machine must have access to pull the images from GCR, or appropriate credentials must be specified in the google.cloud.lifesciences.v2beta.Action.credentials field.
  * labels `object`: Labels to associate with the action. This field is provided to assist workflow engine authors in identifying actions (for example, to indicate what sort of action they perform, such as localization or debugging). They are returned in the operation metadata, but are otherwise ignored.
  * mounts `array`: A list of mounts to make available to the action. In addition to the values specified here, every action has a special virtual disk mounted under `/google` that contains log files and other operational components. - /google/logs All logs written during the pipeline execution. - /google/logs/output The combined standard output and standard error of all actions run as part of the pipeline execution. - /google/logs/action/*/stdout The complete contents of each individual action's standard output. - /google/logs/action/*/stderr The complete contents of each individual action's standard error output. 
    * items [Mount](#mount)
  * pidNamespace `string`: An optional identifier for a PID namespace to run the action inside. Multiple actions should use the same string to share a namespace. If unspecified, a separate isolated namespace is used.
  * portMappings `object`: A map of containers to host port mappings for this container. If the container already specifies exposed ports, use the `PUBLISH_EXPOSED_PORTS` flag instead. The host port number must be less than 65536. If it is zero, an unused random port is assigned. To determine the resulting port number, consult the `ContainerStartedEvent` in the operation metadata.
  * publishExposedPorts `boolean`: Exposes all ports specified by `EXPOSE` statements in the container. To discover the host side port numbers, consult the `ACTION_STARTED` event in the operation metadata.
  * runInBackground `boolean`: This flag allows an action to continue running in the background while executing subsequent actions. This is useful to provide services to other actions (or to provide debugging support tools like SSH servers).
  * timeout `string`: The maximum amount of time to give the action to complete. If the action fails to complete before the timeout, it will be terminated and the exit status will be non-zero. The pipeline will continue or terminate based on the rules defined by the `ALWAYS_RUN` and `IGNORE_EXIT_STATUS` flags.

### CancelOperationRequest
* CancelOperationRequest `object`: The request message for Operations.CancelOperation.

### ContainerKilledEvent
* ContainerKilledEvent `object`: An event generated when a container is forcibly terminated by the worker. Currently, this only occurs when the container outlives the timeout specified by the user.
  * actionId `integer`: The numeric ID of the action that started the container.

### ContainerStartedEvent
* ContainerStartedEvent `object`: An event generated when a container starts.
  * actionId `integer`: The numeric ID of the action that started this container.
  * ipAddress `string`: The public IP address that can be used to connect to the container. This field is only populated when at least one port mapping is present. If the instance was created with a private address, this field will be empty even if port mappings exist.
  * portMappings `object`: The container-to-host port mappings installed for this container. This set will contain any ports exposed using the `PUBLISH_EXPOSED_PORTS` flag as well as any specified in the `Action` definition.

### ContainerStoppedEvent
* ContainerStoppedEvent `object`: An event generated when a container exits.
  * actionId `integer`: The numeric ID of the action that started this container.
  * exitStatus `integer`: The exit status of the container.
  * stderr `string`: The tail end of any content written to standard error by the container. If the content emits large amounts of debugging noise or contains sensitive information, you can prevent the content from being printed by setting the `DISABLE_STANDARD_ERROR_CAPTURE` flag. Note that only a small amount of the end of the stream is captured here. The entire stream is stored in the `/google/logs` directory mounted into each action, and can be copied off the machine as described elsewhere.

### DelayedEvent
* DelayedEvent `object`: An event generated whenever a resource limitation or transient error delays execution of a pipeline that was otherwise ready to run.
  * cause `string`: A textual description of the cause of the delay. The string can change without notice because it is often generated by another service (such as Compute Engine).
  * metrics `array`: If the delay was caused by a resource shortage, this field lists the Compute Engine metrics that are preventing this operation from running (for example, `CPUS` or `INSTANCES`). If the particular metric is not known, a single `UNKNOWN` metric will be present.
    * items `string`

### Disk
* Disk `object`: Carries information about a disk that can be attached to a VM. See https://cloud.google.com/compute/docs/disks/performance for more information about disk type, size, and performance considerations.
  * name `string`: A user-supplied name for the disk. Used when mounting the disk into actions. The name must contain only upper and lowercase alphanumeric characters and hyphens and cannot start with a hyphen.
  * sizeGb `integer`: The size, in GB, of the disk to attach. If the size is not specified, a default is chosen to ensure reasonable I/O performance. If the disk type is specified as `local-ssd`, multiple local drives are automatically combined to provide the requested size. Note, however, that each physical SSD is 375GB in size, and no more than 8 drives can be attached to a single instance.
  * sourceImage `string`: An optional image to put on the disk before attaching it to the VM.
  * type `string`: The Compute Engine disk type. If unspecified, `pd-standard` is used.

### Empty
* Empty `object`: A generic empty message that you can re-use to avoid defining duplicated empty messages in your APIs. A typical example is to use it as the request or the response type of an API method. For instance: service Foo { rpc Bar(google.protobuf.Empty) returns (google.protobuf.Empty); } The JSON representation for `Empty` is empty JSON object `{}`.

### Event
* Event `object`: Carries information about events that occur during pipeline execution.
  * containerKilled [ContainerKilledEvent](#containerkilledevent)
  * containerStarted [ContainerStartedEvent](#containerstartedevent)
  * containerStopped [ContainerStoppedEvent](#containerstoppedevent)
  * delayed [DelayedEvent](#delayedevent)
  * description `string`: A human-readable description of the event. Note that these strings can change at any time without notice. Any application logic must use the information in the `details` field.
  * failed [FailedEvent](#failedevent)
  * pullStarted [PullStartedEvent](#pullstartedevent)
  * pullStopped [PullStoppedEvent](#pullstoppedevent)
  * timestamp `string`: The time at which the event occurred.
  * unexpectedExitStatus [UnexpectedExitStatusEvent](#unexpectedexitstatusevent)
  * workerAssigned [WorkerAssignedEvent](#workerassignedevent)
  * workerReleased [WorkerReleasedEvent](#workerreleasedevent)

### ExistingDisk
* ExistingDisk `object`: Configuration for an existing disk to be attached to the VM.
  * disk `string`: If `disk` contains slashes, the Cloud Life Sciences API assumes that it is a complete URL for the disk. If `disk` does not contain slashes, the Cloud Life Sciences API assumes that the disk is a zonal disk and a URL will be generated of the form `zones//disks/`, where `` is the zone in which the instance is allocated. The disk must be ext4 formatted. If all `Mount` references to this disk have the `read_only` flag set to true, the disk will be attached in `read-only` mode and can be shared with other instances. Otherwise, the disk will be available for writing but cannot be shared.

### FailedEvent
* FailedEvent `object`: An event generated when the execution of a pipeline has failed. Note that other events can continue to occur after this event.
  * cause `string`: The human-readable description of the cause of the failure.
  * code `string` (values: OK, CANCELLED, UNKNOWN, INVALID_ARGUMENT, DEADLINE_EXCEEDED, NOT_FOUND, ALREADY_EXISTS, PERMISSION_DENIED, UNAUTHENTICATED, RESOURCE_EXHAUSTED, FAILED_PRECONDITION, ABORTED, OUT_OF_RANGE, UNIMPLEMENTED, INTERNAL, UNAVAILABLE, DATA_LOSS): The Google standard error code that best describes this failure.

### ListLocationsResponse
* ListLocationsResponse `object`: The response message for Locations.ListLocations.
  * locations `array`: A list of locations that matches the specified filter in the request.
    * items [Location](#location)
  * nextPageToken `string`: The standard List next-page token.

### ListOperationsResponse
* ListOperationsResponse `object`: The response message for Operations.ListOperations.
  * nextPageToken `string`: The standard List next-page token.
  * operations `array`: A list of operations that matches the specified filter in the request.
    * items [Operation](#operation)

### Location
* Location `object`: A resource that represents Google Cloud Platform location.
  * displayName `string`: The friendly name for this location, typically a nearby city name. For example, "Tokyo".
  * labels `object`: Cross-service attributes for the location. For example {"cloud.googleapis.com/region": "us-east1"}
  * locationId `string`: The canonical id for this location. For example: `"us-east1"`.
  * metadata `object`: Service-specific metadata. For example the available capacity at the given location.
  * name `string`: Resource name for the location, which may vary between implementations. For example: `"projects/example-project/locations/us-east1"`

### Metadata
* Metadata `object`: Carries information about the pipeline execution that is returned in the long running operation's metadata field.
  * createTime `string`: The time at which the operation was created by the API.
  * endTime `string`: The time at which execution was completed and resources were cleaned up.
  * events `array`: The list of events that have happened so far during the execution of this operation.
    * items [Event](#event)
  * labels `object`: The user-defined labels associated with this operation.
  * pipeline [Pipeline](#pipeline)
  * startTime `string`: The first time at which resources were allocated to execute the pipeline.

### Mount
* Mount `object`: Carries information about a particular disk mount inside a container.
  * disk `string`: The name of the disk to mount, as specified in the resources section.
  * path `string`: The path to mount the disk inside the container.
  * readOnly `boolean`: If true, the disk is mounted read-only inside the container.

### NFSMount
* NFSMount `object`: Configuration for an `NFSMount` to be attached to the VM.
  * target `string`: A target NFS mount. The target must be specified as `address:/mount".

### Network
* Network `object`: VM networking options.
  * network `string`: The network name to attach the VM's network interface to. The value will be prefixed with `global/networks/` unless it contains a `/`, in which case it is assumed to be a fully specified network resource URL. If unspecified, the global default network is used.
  * subnetwork `string`: If the specified network is configured for custom subnet creation, the name of the subnetwork to attach the instance to must be specified here. The value is prefixed with `regions/*/subnetworks/` unless it contains a `/`, in which case it is assumed to be a fully specified subnetwork resource URL. If the `*` character appears in the value, it is replaced with the region that the virtual machine has been allocated in.
  * usePrivateAddress `boolean`: If set to true, do not attach a public IP address to the VM. Note that without a public IP address, additional configuration is required to allow the VM to access Google services. See https://cloud.google.com/vpc/docs/configure-private-google-access for more information.

### Operation
* Operation `object`: This resource represents a long-running operation that is the result of a network API call.
  * done `boolean`: If the value is `false`, it means the operation is still in progress. If `true`, the operation is completed, and either `error` or `response` is available.
  * error [Status](#status)
  * metadata `object`: An Metadata object. This will always be returned with the Operation.
  * name `string`: The server-assigned name for the operation. This may be passed to the other operation methods to retrieve information about the operation's status.
  * response `object`: An Empty object.

### PersistentDisk
* PersistentDisk `object`: Configuration for a persistent disk to be attached to the VM. See https://cloud.google.com/compute/docs/disks/performance for more information about disk type, size, and performance considerations.
  * sizeGb `integer`: The size, in GB, of the disk to attach. If the size is not specified, a default is chosen to ensure reasonable I/O performance. If the disk type is specified as `local-ssd`, multiple local drives are automatically combined to provide the requested size. Note, however, that each physical SSD is 375GB in size, and no more than 8 drives can be attached to a single instance.
  * sourceImage `string`: An image to put on the disk before attaching it to the VM.
  * type `string`: The Compute Engine disk type. If unspecified, `pd-standard` is used.

### Pipeline
* Pipeline `object`: Specifies a series of actions to execute, expressed as Docker containers.
  * actions `array`: The list of actions to execute, in the order they are specified.
    * items [Action](#action)
  * environment `object`: The environment to pass into every action. Each action can also specify additional environment variables but cannot delete an entry from this map (though they can overwrite it with a different value).
  * resources [Resources](#resources)
  * timeout `string`: The maximum amount of time to give the pipeline to complete. This includes the time spent waiting for a worker to be allocated. If the pipeline fails to complete before the timeout, it will be cancelled and the error code will be set to DEADLINE_EXCEEDED. If unspecified, it will default to 7 days.

### PullStartedEvent
* PullStartedEvent `object`: An event generated when the worker starts pulling an image.
  * imageUri `string`: The URI of the image that was pulled.

### PullStoppedEvent
* PullStoppedEvent `object`: An event generated when the worker stops pulling an image.
  * imageUri `string`: The URI of the image that was pulled.

### Resources
* Resources `object`: The system resources for the pipeline run. At least one zone or region must be specified or the pipeline run will fail.
  * regions `array`: The list of regions allowed for VM allocation. If set, the `zones` field must not be set.
    * items `string`
  * virtualMachine [VirtualMachine](#virtualmachine)
  * zones `array`: The list of zones allowed for VM allocation. If set, the `regions` field must not be set.
    * items `string`

### RunPipelineRequest
* RunPipelineRequest `object`: The arguments to the `RunPipeline` method. The requesting user must have the `iam.serviceAccounts.actAs` permission for the Cloud Life Sciences service account or the request will fail.
  * labels `object`: User-defined labels to associate with the returned operation. These labels are not propagated to any Google Cloud Platform resources used by the operation, and can be modified at any time. To associate labels with resources created while executing the operation, see the appropriate resource message (for example, `VirtualMachine`).
  * pipeline [Pipeline](#pipeline)

### RunPipelineResponse
* RunPipelineResponse `object`: The response to the RunPipeline method, returned in the operation's result field on success.

### Secret
* Secret `object`: Holds encrypted information that is only decrypted and stored in RAM by the worker VM when running the pipeline.
  * cipherText `string`: The value of the cipherText response from the `encrypt` method. This field is intentionally unaudited.
  * keyName `string`: The name of the Cloud KMS key that will be used to decrypt the secret value. The VM service account must have the required permissions and authentication scopes to invoke the `decrypt` method on the specified key.

### ServiceAccount
* ServiceAccount `object`: Carries information about a Google Cloud service account.
  * email `string`: Email address of the service account. If not specified, the default Compute Engine service account for the project will be used.
  * scopes `array`: List of scopes to be enabled for this service account on the VM, in addition to the cloud-platform API scope that will be added by default.
    * items `string`

### Status
* Status `object`: The `Status` type defines a logical error model that is suitable for different programming environments, including REST APIs and RPC APIs. It is used by [gRPC](https://github.com/grpc). Each `Status` message contains three pieces of data: error code, error message, and error details. You can find out more about this error model and how to work with it in the [API Design Guide](https://cloud.google.com/apis/design/errors).
  * code `integer`: The status code, which should be an enum value of google.rpc.Code.
  * details `array`: A list of messages that carry the error details. There is a common set of message types for APIs to use.
    * items `object`
  * message `string`: A developer-facing error message, which should be in English. Any user-facing error message should be localized and sent in the google.rpc.Status.details field, or localized by the client.

### UnexpectedExitStatusEvent
* UnexpectedExitStatusEvent `object`: An event generated when the execution of a container results in a non-zero exit status that was not otherwise ignored. Execution will continue, but only actions that are flagged as `ALWAYS_RUN` will be executed. Other actions will be skipped.
  * actionId `integer`: The numeric ID of the action that started the container.
  * exitStatus `integer`: The exit status of the container.

### VirtualMachine
* VirtualMachine `object`: Carries information about a Compute Engine VM resource.
  * accelerators `array`: The list of accelerators to attach to the VM.
    * items [Accelerator](#accelerator)
  * bootDiskSizeGb `integer`: The size of the boot disk, in GB. The boot disk must be large enough to accommodate all of the Docker images from each action in the pipeline at the same time. If not specified, a small but reasonable default value is used.
  * bootImage `string`: The host operating system image to use. Currently, only Container-Optimized OS images can be used. The default value is `projects/cos-cloud/global/images/family/cos-stable`, which selects the latest stable release of Container-Optimized OS. This option is provided to allow testing against the beta release of the operating system to ensure that the new version does not interact negatively with production pipelines. To test a pipeline against the beta release of Container-Optimized OS, use the value `projects/cos-cloud/global/images/family/cos-beta`.
  * cpuPlatform `string`: The CPU platform to request. An instance based on a newer platform can be allocated, but never one with fewer capabilities. The value of this parameter must be a valid Compute Engine CPU platform name (such as "Intel Skylake"). This parameter is only useful for carefully optimized work loads where the CPU platform has a significant impact. For more information about the effect of this parameter, see https://cloud.google.com/compute/docs/instances/specify-min-cpu-platform.
  * disks `array`: The list of disks to create and attach to the VM.
    * items [Disk](#disk)
  * dockerCacheImages `array`: The Compute Engine Disk Images to use as a Docker cache. The disks will be mounted into the Docker folder in a way that the images present in the cache will not need to be pulled. The digests of the cached images must match those of the tags used or the latest version will still be pulled. The root directory of the ext4 image must contain `image` and `overlay2` directories copied from the Docker directory of a VM where the desired Docker images have already been pulled. Only a single image is supported.
    * items `string`
  * enableStackdriverMonitoring `boolean`: Whether Stackdriver monitoring should be enabled on the VM.
  * labels `object`: Optional set of labels to apply to the VM and any attached disk resources. These labels must adhere to the [name and value restrictions](https://cloud.google.com/compute/docs/labeling-resources) on VM labels imposed by Compute Engine. Labels keys with the prefix 'google-' are reserved for use by Google. Labels applied at creation time to the VM. Applied on a best-effort basis to attached disk resources shortly after VM creation.
  * machineType `string`: Required. The machine type of the virtual machine to create. Must be the short name of a standard machine type (such as "n1-standard-1") or a custom machine type (such as "custom-1-4096", where "1" indicates the number of vCPUs and "4096" indicates the memory in MB). See [Creating an instance with a custom machine type](https://cloud.google.com/compute/docs/instances/creating-instance-with-custom-machine-type#create) for more specifications on creating a custom machine type.
  * network [Network](#network)
  * nvidiaDriverVersion `string`: The NVIDIA driver version to use when attaching an NVIDIA GPU accelerator. The version specified here must be compatible with the GPU libraries contained in the container being executed, and must be one of the drivers hosted in the `nvidia-drivers-us-public` bucket on Google Cloud Storage.
  * preemptible `boolean`: If true, allocate a preemptible VM.
  * serviceAccount [ServiceAccount](#serviceaccount)
  * volumes `array`: The list of disks and other storage to create or attach to the VM.
    * items [Volume](#volume)

### Volume
* Volume `object`: Carries information about storage that can be attached to a VM.
  * existingDisk [ExistingDisk](#existingdisk)
  * nfsMount [NFSMount](#nfsmount)
  * persistentDisk [PersistentDisk](#persistentdisk)
  * volume `string`: A user-supplied name for the volume. Used when mounting the volume into `Actions`. The name must contain only upper and lowercase alphanumeric characters and hyphens and cannot start with a hyphen.

### WorkerAssignedEvent
* WorkerAssignedEvent `object`: An event generated after a worker VM has been assigned to run the pipeline.
  * instance `string`: The worker's instance name.
  * machineType `string`: The machine type that was assigned for the worker.
  * zone `string`: The zone the worker is running in.

### WorkerReleasedEvent
* WorkerReleasedEvent `object`: An event generated when the worker VM that was assigned to the pipeline has been released (deleted).
  * instance `string`: The worker's instance name.
  * zone `string`: The zone the worker was running in.

