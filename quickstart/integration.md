## Creating an Integration

The process for creating a new partner integration is described in detail in the [Adobe I/O documentation](https://www.adobe.io/authentication/auth-methods.html#!AdobeDocs/adobeio-auth/master/AuthenticationOverview/OAuthIntegration.md). A brief outline of the steps is:

1. Identify an existing Adobe ID with an affiliated email address, or create a new one, to use for managing the integration. This Adobe ID will have administrative privileges for the lifecycle of the integration. Log into the Adobe I/O console at: <a href="https://console.adobe.io" target="_blank">https://console.adobe.io</a>.

2. Once logged into the console, select "Create Integration", "Access an API", and "Continue".

3. Under the "Creative Cloud" offerings, select "Lightroom Services" and "Continue". Fill in the form with details to create the integration. Provide redirect URL details here for the OAuth workflow.

4. Once the integration has been created, click on "Integration Details" to identify the API key and client secret. Take note of these values. These details will be needed in generating authorization code. If needed, the integration details such as name, description, and redirect URLs can be modified here. 

5. Once the API key is given access to use the Lightroom Services the approval process is complete. At this point verify access to the APIs through the health check endpoint `/v2/health` with the `X-API-Key` header set the the API key from the previous step.