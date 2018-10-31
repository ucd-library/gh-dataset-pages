# gh-dataset-pages
Create a hosted GitHub/Jekyll website for a GitHub data repository with proper schema.org dataset SEO markup

# Create Website

First ```cd``` to your data repository on your local computer

```bash
cd ~/my-data-repo
```

Now create a new branch called ```gh-pages```

```bash
git checkout -b gh-pages
```

Pull the latest release for this repository, unzip, extract the template and cleanup.
Copy and paste entire code block below.

```bash
wget https://github.com/ucd-library/gh-dataset-pages/archive/master.zip && \
  unzip master.zip && \
  cp -r gh-dataset-pages-master/template/* . && \
  rm -rf master.zip gh-dataset-pages-master
```

Edit the ```_config.yml``` file properties under the section ```Fill out dataset variables below```

```yaml
author:
  name: 
  email: 
keywords:
  - 
genre:
publisher:
  name: 
  url: 
  description: 
datePublished: 
```

Edit the ```index.md``` file and add content for your website

Push new branch to GitHub and set upstream tracking

```bash
git push --set-upstream origin gh-pages
```

Visit your new dataset website host by GitHub!

```bash
https://[[org/username]].github.io/[[respositoryName]]/
```