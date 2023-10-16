# relearnhugo

Sample site practice using HUGO as hosting website for posts and blogs. Users would save time publishing posts by onnly need to use markdown files instead of html and css. 

Sample look
![image](https://github.com/mari1li/relearnhugo/assets/77930939/28d7d81f-d6b0-4412-ab2e-e60b1a9e9907)

Credits to [Relearn Hugo Theme](https://mcshelby.github.io/hugo-theme-relearn/more/credits/index.html)


Notes for implementing website:
disable footer: "Built with Hugo": Find at file /themes/relearn-theme/partials/menu-footer.html

tag button on side bar: go to hugo.toml add 
[[menu.shortcuts]]
name = "<i class='fas fa-tags'></i> Tags"
url = "/tags"

Language implement: hugo.toml disable footer: "Built with Hugo": Find at file /themes/relearn-theme/partials/menu-footer.html

tag button on side bar: go to hugo.toml add 
[languages]
[languages.en]

weight = 1
languageName = "English"
[languages.en.params]
landingPageName = "<i class='fas fa-home'></i> Home"

change theme color: in hugo.toml under [params] add
Change default color scheme with a variant one.
themeVariant = [ "relearn-light", "relearn-dark", "zen-light", "zen-dark", "blue" ]

enable table of content: add this in hugo.toml under [params]
disableToc = false

change logo image: Create a new file in layouts/partials/ (in at the same level as content folder) named logo.html. Then write any HTML you want. You could use an img HTML tag and reference an image then add tag:
<img src="/images/kafka_logo.png" alt="" height=100px>
