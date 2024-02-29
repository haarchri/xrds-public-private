
1. create private api xrds in apis/private
2. run make crds
    this code is copied from crossplane repo a while a go, we need this because crossplane have this functionality in internal folder -> needs updates
    the idea here is to generate from a xrd and crd

3. write generate.yaml in apis/public folder
4. make generate
    we will use as basis the crds from private api and generate our public xrd and composition 

