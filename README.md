# DRU8DnvU
 Version control for our Zotero group DRU8DnvU

 In order to query the XML for a specific title, use the following XPath expression

```xml
//div/head/title[@level = 'j'][contains(., 'البل')]
```

# terminology

+ *ṣāḥib*: owner, concessionary, publisher
    * verbs indicating founders / owners: *aṣdara*
+ *munshiʾ*: "publisher"
+ *mudīr masʾūl*: responsible editor, director responsible, director-in-charge
    * there seems to be no clear equivalent outside the former Ottoman realms
    * it is still used in Arabic and Turkish
+ *raʾis al-taḥrīr*: editor-in-chief (wikipedia), Rédacteur en chef (wikipedia)
+ *mudīr al-taḥrīr*: managing editor
+ *muḥarrir*: editor

- how to encode these roles in TEI?
    + `@type` on `<editor>`! i.e. `<editor type="owner"/>`
        * owner: *ṣāḥib*,
        * publisher: *nashaʾa*, *aṣdara*, *nashara*
        * editor: *ḥarrara* (implicitly assumed)
            - editor-in-chief
            - managing-editor
            - editor