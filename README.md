# sofistik-tools

<p align="center">
  <img src="https://img.shields.io/github/v/tag/bacadra/atom-sofistik-tools?style=for-the-badge&label=Latest&color=007EC6" alt="Latest">
  <img src="https://img.shields.io/github/languages/code-size/bacadra/atom-sofistik-tools?style=for-the-badge&color=007EC6" alt="CodeSize">
  <img src="https://img.shields.io/github/languages/top/bacadra/atom-sofistik-tools?style=for-the-badge&color=007EC6" alt="Language">
  <img src="https://img.shields.io/github/last-commit/bacadra/atom-sofistik-tools?style=for-the-badge&color=007EC6" alt="LastCommit">
  <img src="https://img.shields.io/github/license/bacadra/atom-sofistik-tools?style=for-the-badge&color=007EC6" alt="Licence">
</p>

A set of tools for cooperation with the SOFiSTiK software.

## Installation

### Atom Text Editor

The official Atom packages store has been disabled. To get latest version run the shell command

    apm install bacadra/atom-sofistik-tools

and obtain the package directly from Github repository.

### Pulsar Text Editor

The package has compability with [Pulsar](https://pulsar-edit.dev/) and can be install

    pulsar -p install bacadra/atom-sofistik-tools

or directly [sofistik-tools](https://web.pulsar-edit.dev/packages/sofistik-tools) from Pulsar package store.

## Compatibility

<%sofistik_compatibility%>

## Configuration

The most important part is to correctly set the software installation path and the SOFiSTiK version. You can do it in package settings.

The package support shebang as regex `^@ SOFiSTiK (\d{4})(-\d\d?)?$`, e.g. `@ SOFiSTiK 2022`, `@ SOFiSTiK 2018`, `@ SOFiSTiK 2018-12`. This overwrite global package settings.

## Help view

The help view can be opened in any internal or external PDF viewers. If [pdf-viewer](https://github.com/bacadra/atom-pdf-viewer) is used, then help PDF file can be scrolled to current keyword.

## Tools available in `source.sofistik` (e.g. `.dat` file)

The tools listed below should be called up via the Command Palette as `SOFiSTiK-tools:...`

| Tool | Description |
|-|-|
| <div style="white-space:nowrap">`current-help`               </div> | open help for current module in Atom in single pane |
| <div style="white-space:nowrap">`current-help-multi`         </div> | open help for current module in Atom, but multi panes |
| <div style="white-space:nowrap">`current-help-externally`    </div> | same as `current-help`, but in externally PDF viewer |
| <div style="white-space:nowrap">`calculation-WPS`            </div> | open WPS with loaded `.dat` file |
| <div style="white-space:nowrap">`calculation-WPS-immediately`</div> | run calculation of file in WPS |
| <div style="white-space:nowrap">`calculation-WPS-current`    </div> | run calculation of current module in WPS |
| <div style="white-space:nowrap">`calculation-SPS-immediately`</div> | run calculation of file in SPS |
| <div style="white-space:nowrap">`open-report`                </div> | open `.plb` file with ReportViewer |
| <div style="white-space:nowrap">`open-report-auto-refresh`   </div> | open `.plb` file with ReportViewer with flag to automatically refresh file if changed |
| <div style="white-space:nowrap">`save-report-as-PDF`         </div> | convert `.plb` to `.pdf` |
| <div style="white-space:nowrap">`save-pictures-as-PDF`       </div> | export images from `.plb` |
| <div style="white-space:nowrap">`open-protocol`              </div> | open protocol document |
| <div style="white-space:nowrap">`open-Animator`              </div> | open `.cdb` in Animator or System Visualization |
| <div style="white-space:nowrap">`open-SSD`                   </div> | open `.sofistik` file in SSD |
| <div style="white-space:nowrap">`open-WinGRAF`               </div> | open `.gra` file with same name as `.dat` file |
| <div style="white-space:nowrap">`open-Result-Viewer`         </div> | open `.result` file with same name as `.dat` file |
| <div style="white-space:nowrap">`open-Teddy`                 </div> | open `.dat` file externally in Teddy |
| <div style="white-space:nowrap">`open-Teddy-single`          </div> | open `.dat` file externally in Teddy |
| <div style="white-space:nowrap">`open-Teddy-1`               </div> | open `.dat` file externally in Teddy in slot 1 |
| <div style="white-space:nowrap">`open-Teddy-2`               </div> | open `.dat` file externally in Teddy in slot 2 |
| <div style="white-space:nowrap">`open-Teddy-3`               </div> | open `.dat` file externally in Teddy in slot 3 |
| <div style="white-space:nowrap">`open-Teddy-4`               </div> | open `.dat` file externally in Teddy in slot 4 |
| <div style="white-space:nowrap">`open-SOFiPLUS`              </div> | open `.dwg` file only if exists else just open program |
| <div style="white-space:nowrap">`export-CDB-to-DAT`          </div> | open export window from `.cdb` to `.dat` |
| <div style="white-space:nowrap">`export-PLB-to-DOCX`         </div> | convert `.plb` file to `.docx`; work only with SOFiSTiK 2020 or higher versions |
| <div style="white-space:nowrap">`PROG-current-toggle`        </div> | toggle state of PROG of current program |
| <div style="white-space:nowrap">`PROG-all-toggle`            </div> | toggle all programs |
| <div style="white-space:nowrap">`PROG-all-ON`                </div> | turn ON all programs |
| <div style="white-space:nowrap">`PROG-all-OFF`               </div> | turn OFF all programs |
| <div style="white-space:nowrap">`PROG-above-toggle`          </div> | toggle programs above cursor |
| <div style="white-space:nowrap">`PROG-above-ON`              </div> | turn ON programs above cursor |
| <div style="white-space:nowrap">`PROG-above-OFF`             </div> | turn OFF programs above cursor |
| <div style="white-space:nowrap">`PROG-below-toggle`          </div> | toggle programs below cursor |
| <div style="white-space:nowrap">`PROG-below-ON`              </div> | turn ON programs below cursor |
| <div style="white-space:nowrap">`PROG-below-OFF`             </div> | turn OFF programs below cursor |

## Tools available in `atom-workspace`

The tools listed below should be called up via the Command Palette as `SOFiSTiK-tools:...`

| Tool | Description |
|-|-|
| <div style="white-space:nowrap">`open-help`      </div> | open window to choose help document; press `Enter` to open help inside atom or `Alt-Enter` to open externally; open inside atom is possible only with any PDF viewer package |
| <div style="white-space:nowrap">`IFC-export`     </div> | open IFC export window |
| <div style="white-space:nowrap">`IFC-import`     </div> | open IFC import window |
| <div style="white-space:nowrap">`change-version` </div> | change globally version of SOFiSTiK program without menu |
| <div style="white-space:nowrap">`open-CDBASE.CHM`</div> | open database description externally; `.chm` browser must be available in system |
| <div style="white-space:nowrap">`open-SOFiPLUS`  </div> | open program |

## Tools available in `.tree-view`

The tools listed below should be called up via the Command Palette as `SOFiSTiK-tools:...`

| Tool | Description |
|-|-|
| `clean-[S]-[ERG-PRT-LST-URS-SDB-DB2-PL-$??-#??-GRB]` | delete files only in selected paths |
| `clean-[R]-[ERG-PRT-LST-URS-SDB-DB2-PL-$??-#??-GRB]` | delete files recursively from selected paths |
| `clean-[S]-[ERG-PRT-LST-URS-SDB-DB2-PL-$??-#??-GRB-CDI-CDE]` | delete files only in selected paths |
| `clean-[R]-[ERG-PRT-LST-URS-SDB-DB2-PL-$??-#??-GRB-CDI-CDE]` | delete files recursively from selected paths |
| `clean-[S]-[ERG-PRT-LST-URS-SDB-DB2-PL-$??-#??-GRB-CDI-CDE-CDB-PLB-BAK-SDB-DOCX-CFG-CSM]` | delete files only in selected paths |
| `clean-[R]-[ERG-PRT-LST-URS-SDB-DB2-PL-$??-#??-GRB-CDI-CDE-CDB-PLB-BAK-SDB-DOCX-CFG-CSM]` | delete files recursively from selected paths |

# Contributing

If you have ideas on how to improve the package, see bugs or want to support new features - feel free to share it via GitHub.

See my other packages for Atom & Pulsar Text Editors:

* [autocomplete-sofistik](https://github.com/bacadra/atom-autocomplete-sofistik)
* [bib-finder](https://github.com/bacadra/atom-bib-finder)
* [hydrogen-run](https://github.com/bacadra/atom-hydrogen-run)
* [image-paste](https://github.com/bacadra/atom-image-paste)
* [language-sofistik](https://github.com/bacadra/atom-language-sofistik)
* [linter-ruff](https://github.com/bacadra/atom-linter-ruff)
* [navigation-panel](https://github.com/bacadra/atom-navigation-panel)
* [open-external](https://github.com/bacadra/atom-open-external)
* [pdf-viewer](https://github.com/bacadra/atom-pdf-viewer)
* [project-files](https://github.com/bacadra/atom-project-files)
* [regex-aligner](https://github.com/bacadra/atom-regex-aligner)
* [sofistik-tools](https://github.com/bacadra/atom-sofistik-tools)
* [super-select](https://github.com/bacadra/atom-super-select)
* [word-map](https://github.com/bacadra/atom-word-map)
