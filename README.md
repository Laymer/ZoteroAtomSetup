# ZoteroAtomSetup
Attempt towards a setup guide for Zotero bibliography tool combined with a Git repository and plugged with Atom editor

## Installing Zotero

The [Zotero](https://www.zotero.org) standalone software must be installed in order to store references on the local host. It will enable all the functions described below.

## Zotero connectors

Once the Zotero software is installed, it can be combined with [Zotero Connectors](https://www.zotero.org/download/connectors) for Web browsers in order to automatically retrieve data from online references. The Zotero software must be running for the connectors to be able to function. 

### Saving references 

#### Creating a collection

It is usually useful to create a collection in your Zotero library beforehand to organize saved references into different folders. Zotero references can be thought of as Web bookmarks. The Zotero library contains all the bookmarks, and Zotero collections are the equivalent of subfolders for bookmarks. Creating a collection is done in Zotero as follows :

<p align="center">
  <img src="http://g.recordit.co/ekhUQA6l0x.gif" alt="Creating a collection"/>
</p>

#### Saving references from the browser

While having the Zotero software running and once the browser connector has been installed, a reference can be saved into a collection using the following shortcut or clicking on the Zotero button in the browser toolbar when the reference's web page is visited :

```
CTRL + SHIFT + S (Windows)
CMD + SHIFT + S (Mac OS) 
```
:warning: The Mac OS shortcut is not supported in Safari, since it is used to actually bookmark the page. Safari users should therefore simply click on the Zotero connector button. 

It will display a dialog box where the target collection can be set. Zotero will automatically retrieve all available data/metadata such as PDF, links and abstract and store it locally, as shown below :

<p align="center">
  <img src="http://g.recordit.co/u8x9xorovt.gif" alt="Saving a reference"/>
</p>

## The Better BibTeX extension

[Better BibTeX](https://retorque.re/zotero-better-bibtex/) can be used to extend the Zotero software to enable it to automatically export collections as `.bib` files and create citation keys that can be used in LaTeX files with `\cite{articleKey}` to cite the references that have been previously stored. 

Installing the Better BibTeX plug-in is necessary in order to be able to use the Atom package described below.

## Zotero-picker

[Zotero-picker](https://atom.io/packages/zotero-picker) makes it possible to easily cite the references using the citation keys created by Better BixTeX. Once the package is installed, `ALT + Z` should display a Zotero search bar that allows the user to browse his references and retrieve their citation key. 

NOTE : the `@` prefix that is automatically added to the citation key should be removed for the `\cite{reference}` command.

<p align="center">
  <img src="http://g.recordit.co/z1ar8hovSN.gif" alt="Citing a reference in Atom"/>
</p>
