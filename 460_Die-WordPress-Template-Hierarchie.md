# Die WordPress Template Hierarchie

Which template file will wordpress use?
Welche Template-Datei wird WordPress verwenden?

## Template Hierarchie
|============|================================================|
| Seiten Typ | Suchreihenfolge[^suchreihenfolge-child-eltern] |
|============|================================================|
| 404        | 404.php → index.php                            |
|------------|------------------------------------------------|
| SEARCH     | search.php → index.php                         |
|------------|------------------------------------------------|
| TAXONOMY   | taxonomy-{tax}-{term}.php → taxonomy-{tax}.php |
|            | → taxonomy.php → archive.php → index.php       |
|------------|------------------------------------------------|
| HOME       | home.php[^bloghome] or front-page.php[^pagehome] → index.php  |
|------------|------------------------------------------------|
| ATTACHMENT | {mimetype}.php → {subtype}.php → attachment.php|
|            |  → single.php → index.php                      |
|------------|------------------------------------------------|
| SINGLE     | single-{post-type}.php → single.php            |
|            | → singular.php → index.php                     |
|------------|------------------------------------------------|
| PAGE       | {custom-template}.php → page-{slug}.php        |
|            | → page-{id}.php → page.php → singular.php      |
|            | → index.php                                    |
|------------|------------------------------------------------|
| CATEGORY   | category-{slug}.php → category-{id}.php        |
|            | → category.php → archive.php → index.php       |
|------------|------------------------------------------------|
| TAG        | tag-{slug}.php → tag-{id}.php → tag.php        |
|            | → archive.php → index.php                      |
|------------|------------------------------------------------|
| AUTHOR     | author-{author-nicename}.php                   |
|            | → author-{author-id}.php → author.php          |
|            | → archive.php → index.php                      |
|------------|------------------------------------------------|
| DATE       | date.php → archive.php → index.php             |
|------------|------------------------------------------------|
| ARCHIVE    | archive.php → index.php                        |
|============|================================================|


[^suchreihenfolge-child-eltern]: WordPress sucht immer zuerst in einem allfälligen Child Theme, dann im Eltern-Theme
[^bloghome]: Startseite zeigt letzte Beiträge
[^pagehome]: Startseite zeigt eine statische Seite