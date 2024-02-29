

1. Create a private API XRDS within the `apis/private` directory
2. Execute the make crds command. This step is necessary because the functionality to generate from an XRD and a CRD is originally sourced from the Crossplane repository, specifically from an internal folder, and requires updates to match current status.

3. In the `apis/public` folder, create a file named `generate.yaml`
4. Run the `make generate` command. This process will use the CRDs from the private API (located in `package/crds`) as a foundation to generate our public XRDS and compositions. During this generation process, it's possible to:
- Skip and override specific fields according to requirements.
- In future updates, incorporate additional functionalities such as enums, transforms, etc., to enhance the flexibility and utility of the public APIs in https://github.com/crossplane-contrib/x-generation




