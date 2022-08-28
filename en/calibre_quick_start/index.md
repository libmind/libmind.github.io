# Calibre Quick Start Guide


## Introduction

Calibre is an open source e-book management tool. Simply put, calibre allows you to organize your e-book library, convert e-books to various formats, and interact with your e-book reader, all in an intuitive and friendly manner. It is compatible with Microsoft Windows 8 onwards – as well as Apple’s macOS (and various flavors of Linux). It was created by Kovid Goyal, who still leads its development. A number of people around the world, including myself, contribute to calibre’s development. Throughout this guide and the online docs you will see ‘calibre’ instead of ‘Calibre’. That’s the convention Kovid chose, so that’s what we use.

The purpose of calibre is to simplify management of your e-book library. It does this in several ways:

- Calibre organizes your library as a database so you can find the book you want when you want it. Calibre easily handles any size of library, and can manipulate e-book metadata – title, author, rating, etc..

- Calibre converts between multiple e-book formats.

- Calibre supports a growing number of e-book readers, including Kindle, Kobo, Nook, and many others.

Calibre is composed of three functional groups:

- The graphical user interface (GUI). This is the typical mode of interacting with your library. All of calibre’s principal functionality is available through the GUI.

- A collection of command line (CLI) utilities for advanced calibre operations. For example, the command line tools are used by the ManyBooks service to convert on an as-needed basis.

- Additional GUI tools such as an e-book reader and an e-book editor. These tools can be accessed via the main GUI or directly.


## Installing calibre

The installation processes starts by downloading the installer for your operating system. Run the installer; when it finishes, launch calibre. You will be greeted with a welcome wizard, that will help you initially configure calibre. The first page of the wizard allows you to choose the storage location for your e-book library.

If this is your first time using calibre, the storage location should not be an existing e-book collection, but a new empty directory for calibre’s exclusive use. Calibre manages the e-books you give it in its own way. Think of the storage location as a black box. You don’t do anything with it – calibre manages the storage location for you. If you have used calibre in the past and are installing a new version, or if you have moved your library, then it’s okay to indicate a directory with an existing calibre library. Calibre is smart enough to know to use an existing library when it sees one.

Click ‘next’ in the welcome wizard to be presented with an e-book reader selection. If your device is not listed, or if you intend to use more than one e-book reader, don’t panic – just use the default ‘Generic’ choice. This selection provides some conversion optimization for formats requiring fixed sizes. Click ‘next’ and then ‘finish’.

Congratulations, you’ve successfully installed and configured calibre! If at any time you want to run the welcome wizard again, click the downward facing arrow to the right of the Preferences button (looks like a set of three gears) in the top tool bar, then select ‘Run welcome wizard’.


## The Main Library Window, aka the GUI

Once the welcome wizard finishes you will be presented with the main application window. There are a few components I would like to bring to your attention. The central piece is the book list. This takes up the majority of the window and displays the books in a table. Just above the book list you will see the search area (more on this later) and above that, the tool bar. When you connect a supported e-book reader a ‘Device’ icon will appear next to the ’Library’ icon in the tool bar. You can switch between viewing books in your library and books on your e-book reader by clicking on their respective icons.

The panel along the right of the window shows details about the currently selected book, including its cover. If you double click anywhere in the detail area (including on the book cover) another window will open exposing more information about the book. Clicking on any blue text in this area will perform an action specific to the information. For example, clicking the author’s name will open your web browser and search Wikipedia for information about the author.

At the bottom right of the window there are four icons and the word “Jobs”. Clicking any of these icons will toggle a given view state in the GUI. From left to right:

- The luggage tag toggles the tag browser (on the left of the window). More on this later.
- The curved arrow toggles the cover flow display. Cover flow displays the book covers in a fashion similar to how a juke box lays out albums. The selected book is in the center while the neighboring covers are shown at an angle. You can navigate though the book covers with the left and right arrow keys on your keyboard. The book list will still be visible under the cover flow area.
- The nine squares in a grid toggles cover grid view. The cover grid replaces the book list with a grid of book covers. You might want to think of this as bookshelf view.
- The book toggles seeing the details panel on the right.
- The jobs indicator is one of the most important pieces of the GUI. This is the word ‘Jobs:’, the number next to it and the circular progress indicator. Whenever calibre is working on something (conversion, sending books to the reader, downloading news, etc.) the circular icon will spin and the number will reflect the number of jobs (activities) calibre is working on. You can click any part of the jobs indicator to show more detail about the jobs in progress.

## Common Tasks

Let’s take a look at a few of the common tasks people use calibre for:

1. [Organizing your e-book library](javascript:void(0))
2. [Conversion](javascript:void(0))
3. [Editing e-books](javascript:void(0))
4. [Downloading news from websites](javascript:void(0))
5. [Dealing with devices](javascript:void(0))
6. [Viewing e-books](javascript:void(0))

### Task 1: Organizing

The first part of organizing is getting your e-books into calibre’s library. Click the ‘Add books’ button in the tool bar at the top of the window, then select the e-books you would like calibre to import. When calibre imports your e-books it makes a copy of them in the storage location you specified during initial setup. Once you’ve added an e-book, calibre doesn’t need further access to the original file.

During an e-book import, calibre tries to read the metadata from the e-book. Metadata is information about the book that is stored within the e-book itself. Different formats support different information. Often the information is incomplete or just plain wrong. Don’t worry – calibre makes it easy to fix this. Select the book whose metadata you want to change by clicking the book title in the main window. Then click ‘Edit metadata’ on the top tool bar (to the right of the ‘Add books’ button) and the metadata editor will open.

The easy way to correct the metadata is to fill in the title and author, then click the ‘Download metadata’ button at the bottom, center of the Edit metadata dialog. Calibre will display possible matches for the information entered. If there is more than one result select the entry that looks like the best match. A lot of information should be filled in now.

Above the ‘Download metadata’ button and to the top, right of the cover image is the ‘Download cover’ button. If the book doesn’t have a cover showing or if you don’t like the cover, click it to try to have calibre download one from the internet.

Now that you have your e-books in calibre there are a few different ways to find specific e-books in your library. Direct Searching is one of the fastest ways. Above the book list there is a Search field. Think of it like having Google built into calibre. Just type a few key words into the Search field. Try the author, title, series, or anything else from the e-book’s metadata. E-books matching your search terms are shown as filtered results. The other e-books are still in your library, but they won’t be shown if the search expression doesn’t find them.

You can also use the tag browser to search your library. Along the left side of the window is the tag browser. If you don’t see anything to the left of the book list, click the luggage tag icon in the lower right of the main window; a list will appear to the left of the library. It allows you to see specific subsets of your library. Clicking the icon to the left of each tag allows you to display just the e-books matching that criteria. A plus searches for all books that match and a minus searches for all books that don’t match. Notice that as you enable items in the tag browser search queries are added to the Search field. The tag browser is really just an easy way to create search queries. You could type the query directly into the Search field and see the same result.

### Task 2: Conversion

This is arguably the most useful, and most complex, feature calibre offers. Three of the most popular e-book readers today are the Amazon Kindle, the Kobo and the Barnes & Noble Nook. Unfortunately, not all of these devices read the same kinds of e-books. This mess is like the one in the music world where you might find such formats as WMA, MP3 and AAC. In e-books, the same confusion exists—the Tower of eBabel, as some call it.

#### 2.1: Background

If you are only buying e-books from the store associated with your reader—for example, Amazon’s Kindle Store or Kobo’s Store—you don’t need to worry about any of this. But there are very good reasons why you should know about the major formats, what formats your reader supports, and how to convert between formats.

In addition to the big e-books stores, many online sites offer e-books. Everything from public domain works to novels (often offered at no charge) by well known and lesser known authors. The ‘Get books’ icon in the toolbar allows you to easily comparison shop via a store search dialog. This allows you to search many different stores (uncheck or check the stores you want it to use on the left), big and small, at once. It not only helps you find the best price but also the right format for the book you’re looking for. Please note that this feature connects you to a third party, the store, so any issues related to a purchase should be directed to the store itself because calibre is not part of this exchange.

Often you can download e-books in a variety of formats, but you won’t always find them in a format your e-book reader supports. Here is where conversion comes in. There is a very good chance that you will be able to take an e-book and convert it to a format your reader supports. Realize that you can’t convert e-books that use [Digital Rights Management](https://www.teleread.com/drm/drm-a-teleread-primer/) (DRM).

In the rest of the conversion section I will focus on three devices. 1) The Amazon Kindle which supports the AZW3 format. 2) The Kobo, which supports the EPUB format. 3) The Barnes & Noble Nook, which also supports the EPUB format. While both the Kobo and Nook use the EPUB format, books purchased from one store may not be readable on another device due to DRM.

#### 2.2: Why are there different e-book formats?

Advances in technology is one reason why so many different e-book formats exist. In fact, it’s a major reason. Just like the transition from VHS to DVD and now to Blu-Ray, older formats which were created to solve the problems faced at that time are replaced with newer formats that better meet the needs of today. A great example of this is the e-books people read back in the ’90s on their PDAs. Those devices were very limited in what they could display. E-book readers today are much more advanced. They can display large images and handle advanced formatting. These newer devices needed updated formats that could provide these features.

E-book formats are constantly evolving. While new formats aren’t introduced very often, existing formats (like EPUB) are constantly being updated. For example, the transition from EPUB 2 to EPUB 3. One big change that comes with EPUB 3 is the ability for EPUB to support audio and video. While supporting audio and video might seem counter intuitive for an e-*book*, it make sense when you think about e-books as rich media. Coupled with a tablet or phone, audio and video can work very well and greatly enhance the readers experience.

Another major reason for the proliferation of e-book formats is exclusivity. Many vendors like to control their own proprietary format so they are not dependent on outside companies. They also have the benefit of being able to license their format for use by others. Finally, controlling the format allows them to lock users into their platform. E-books, being relatively new, are undergoing the same growing pains that Betamax and VHS or HD-DVD and Blu-Ray went though. The EPUB format, from the International Digital Publishing Forum (IDPF), is an industry standard intended to reduce these problems.

#### 2.3: Conversion basics

The first thing you need to do is find out what formats your e-book reader supports. The Kindle supports AZW3, MOBI, PRC, AZW1, TPZ, PDF and TXT. The Kobo supports EPUB, PDF, MOBI, RTF, CBZ, CBR, and TXT. The Nook supports EPUB, and PDF. Don’t let this scare or confuse you; all of the major e-book readers support multiple formats. Even with this jumble of letters, you only need to worry about the preferred format for the e-book reader. This preferred format is the one that gives the best formatting. As I mentioned earlier for the Kindle, you really only need to worry about AZW3. For the Kobo and Nook you only need to worry about EPUB. However, it is a good idea to be aware of all of the supported formats because it wouldn’t make sense to convert a MOBI to AZW3 for reading on your Kindle because the Kindle can already read MOBI. Conversion is only necessary to fill in the gaps. For example, if you want to read an EPUB on your Kindle you can convert the EPUB to AZW3.

#### 2.4: Auto conversion

Auto converting e-books with calibre is simple and straightforward:

1. Open Calibre and select the e-book to convert in the library list.
2. Connect your e-book reader to your computer. Calibre will take a moment to detect and scan your e-book reader.
3. Click the ‘Send to device’ button in the top tool bar.
4. Calibre is smart enough to know if the book is in a format supported by your reader. If it’s not, calibre will ask you if you want to auto convert. Say yes, and calibre will take care of the conversion and put the book on your reader.

That’s all there is to it. Doing it is easier than it sounds because all you need to do is select the book you want on your device and click ‘Send to device.’ Calibre worries about the formats and converting for you.

#### 2.5: More robust conversion

Auto conversion is the easiest way to go and in most cases will be all you need to do. However, there are a large number of options that give you control over the conversion process. Click the ‘Convert books’ button in the top tool bar. This screen looks very complicated, but realize that the majority of options here don’t need to be changed from the default. Most of the options only need to be changed in special cases. There is one option that is very important and may need to be changed. At the top right there is a drop down for ‘Output format’. This controls what format the conversion will generate. Kindle owners will select AZW3 while Kobo and Nook owners will select EPUB.

In the conversion dialog there are a few things to check before clicking ‘OK’ to begin the conversion. The first thing you need to do is double check the metadata and make adjustments if necessary. Also, click on ‘Look & Feel’ on the left side. The ‘Remove spacing between paragraphs’ option is very popular. It will cause paragraphs to be formatted with an indent at the beginning instead of separating them with a blank line. It makes the result look more like a printed book than the default, which looks a lot like a web page.

Next, click ‘Page Setup’. If you didn’t select your device during the welcome wizard, you can set it here. The input and output profiles provide specialized optimization for your selected device. Be aware that not all formats are affected by the profile.

That’s it for the basic conversion options. Every option in the conversion dialog has a description of what it does and is displayed when you hover the mouse cursor over it. Look though the options and play with them to produce output that suits your taste. Options set in the conversion dialog are saved on a per book basis. Each time you click convert for a particular e-book, the options from the last time you converted it will be remembered. However, your changes will not be applied to other e-books in your library.

Clicking ‘OK’ closes the dialog and begins the conversion.

After the conversion is finished (look at the jobs indicator) click the downward facing arrow to the right of the ‘Send to device’ button. Select one of the ‘Send specific format’ options (main memory is usually the best choice). A dialog will appear asking you which format you want to send. Select the format you chose in the conversion options. This allows you to specify what format you want sent to your device. If you don’t explicitly select a format and you just click the ‘Send to device’ button calibre will send the ‘preferred’ format for the connected reader. The preferred format is based on a configurable preference list which is device specific.

#### 2.6: Limitations of conversion

An issue that often arises during conversion is missing or incomplete formatting. Not all e-book formats support the same formatting, so layout details may be lost when converting from one format to another. Formatting attributes, like bold and italics, will be preserved in most cases but complex page layout may not be. AZW3 and EPUB both support complex formatting, so you won’t have to worry about this as much when converting between these formats.

Conversion will only shift what the input provides into another format. It will not add anything that was not already in the input to the output. If the input is poorly formatted, the output will be too.

There are some conversion options, Search & Replace and Heuristic Processing, that allow for some modification of the e-book’s content. These options should be used with care. Since they modify the e-book’s content there is the possibility of losing something by accident. It’s best to avoid these options unless you know what you’re doing.

#### 2.7: DRM: the bane of conversion

DRM is an acronym for Digital Rights Management.

Let’s think about physical books for a moment. With a physical book, you can lend or resell your book. But when you do either, you are without the book. With e-books, that is not necessarily the case. E-books are just files on your computer and they can be copied any number of times and given away any number of times. DRM was designed to prevent unlimited copying of an electronic file. Some e-book reader users would say that it is a handy way for companies to try to lock users into a specific brand.

DRM “enables” (really it disables) various end-user rights as determined by the publisher and seller. Some DRM’d e-books cannot be read on more than one device. Some will allow for only partial copying and printing. Some may even allow for lending, a feature shared with physical books. Simply put, DRM restricts what you can do with your e-book. I believe that Digital *Restrictions* Management is a more sutitable name.

An e-book with DRM cannot be converted to a different format. This is because conversion itself would require the removal of the DRM. Not all e-book formats support DRM and different e-book formats support different DRM restrictions. There is no way to move the DRM with the content when converting; thus DRM prevents conversion.

You might be tempted to look for some way to remove DRM from e-books in order to facilitate conversion. A word of warning about doing this: In the USA there is a law known as the [Digital Millennium Copyright Act](https://en.wikipedia.org/wiki/Dmca) (DMCA). This law makes it illegal to circumvent a copy protection system (DRM is such a copy protection system). It also makes it illegal to produce or distribute tools that aid in circumvention. Not everyone lives in the USA, but many countries have similar laws. Check your local laws and realize that even though you may only want to read an EPUB that you’ve legally purchased on your Kindle, it may not be legal to do so. If you don’t like this silliness—and I don’t—then speak up to whoever in your country makes the relevant laws.

### Task 3: The e-book editor

Calibre includes a tool specifically for editing e-books. The e-book editor supports the EPUB and AZW3 formats. Right click any book in your library and select ‘Edit book’ to open the editor.

The editor is very useful if there are typos you wish to correct or layout changes you’d like to make. It’s invaluable when trying to clean up a book that just won’t convert quite how you want. Don’t be fooled though, the editor isn’t only for simple tasks, it’s capable of handling even the most complex of layouts.

In addition to including the features you’d expect from a text editor (syntax highlighting, line numbers, and regular expression based find/replace) it also supports a large number of features specific to e-books:

- Live preview
- Table of contents editor
- Embedded font support including subsetting
- Smarten punctuation
- Remove unused CSS
- Error checking
- Much, much more

### Task 4: Downloading news

This feature of calibre is often overlooked. Integrated into calibre is the ability to download news from a variety of sources. As of this writing 1543 sources (‘recipes’) from all over the world, including both free and paid content, are supported. The real advantage of having calibre manage your news subscriptions is that once downloaded the content will be formatted for reading on your e-book reader. However, you can still read the news right on your computer. If you’re going to be reading the downloaded news on an e-book reader it’s best to go into ‘Preferences’, select ‘Behavior’ and set the ‘Preferred output format’ in General options to the preferred format for your e-book reader. This would be AZW3 for Kindle, and EPUB for the Kobo and Nook.

Click the ‘Fetch news’ button in the top tool bar to open the news download scheduler. With so many sources the best thing to do is find the ones you like and set them to automatically download at a time convenient for you. If you don’t want to schedule automatic downloads and would rather handle it manually, you can. Just use the ‘Download now’ button that appears when you have selected a news source.

In the news download scheduler you can expand the categories that are relevant to you (the ones in languages you can read) by clicking the disclosure triangles to the left of the language groupings. Look through the entries for something of interest. When you find one, select it and check the ‘Schedule for download’ check box on the right, or click ‘Download now’. You can also set how often and when you want it to download. Once downloaded the content will be converted to an e-book according to your conversion preferences.

By default when you connect your e-book reader calibre will automatically transfer the downloaded news to the device. If you don’t want this to happen, and would rather transfer manually go into the ‘Preferences’, select the ‘Behavior’ category, and uncheck ‘Automatically send downloaded news to ebook reader’. Also, if you do want it send to the reader automatically it’s usually a good idea to check the ‘Delete news from library when automatically sent to reader’ option.

### Task 5: Interacting with e-book readers

In my mind the reason people start reading e-books as opposed to physical books (p-books) is due to e-book readers. That’s precisely why I started collecting e-books. Calibre has full support for a wide variety of e-book readers. In total, calibre currently supports over 40 e-book readers. Yep, over 40. Everything from eInk devices like the Kindle, Kobo and Nook to cell phones and tablets.

#### 5.1: Putting an e-book on your e-book reader

Connect your e-book reader to your computer, and start calibre if it’s not already running. If your device is supported by calibre a ‘Device’ icon will appear next to the ‘Library’ button in the tool bar. Clicking the ‘Device’ icon will switch the book list from your library to a listing of e-books on your connected device. If you want to send an e-book to your device just switch back to your library, select the ‘Library’ and click ‘Send to device’ in the top tool bar. It really is that simple. Another often-used feature is removing e-books from the device by selecting a book on the device and click the ‘Remove books’ button in the top tool bar.

Once you’ve finished managing the e-books stored on your device, click the down arrow next to the ‘Device’ button. You will see an eject icon (upward-pointing triangle inside a circle). Clicking the eject icon disconnects your e-book reader from the computer. Always eject your device before disconnecting it. Bad things can happen if you don’t do this.

#### 5.2: E-book reader optional configuration

There are a number of different ways you can configure calibre to interact with your device, but I’m only going to touch on the two most commonly changed options.

Open up ‘Preferences’ and click ‘Sending books to devices’. Here you can customize the save template to change where e-books are saved on your device. If you have experience with music tagging programs where you can create custom save locations this should look very familiar. If you have a device like the Kindle or Kobo this isn’t very useful and can safely be left with the default settings. If you have a device, like the Cybook Gen 3, that supports folders this is extremely useful. There are a number of variables (descriptions under the template) which can be used to change where the books are saved. Lets look at a basic example, “favorites/{title} – {authors}”. {title} will be replaced with the title of the book, {authors} will be replaced with its author and the book will be put into the favorites folder. All of the replacements that can be made in the save template are listed with descriptions under template field.

Another useful configuration change is disabling and reorganizing the supported formats. Let’s use the Cybook Gen 3 again as an example. In ‘Preferences’, click ‘Plugins’, then go to ‘Device Interface plugins’, select the ‘Cybook Gen 3 / Opus Device Interface’ and click ‘Customize plugin’. In the configuration for the device you will see a e-book format list. Here you can uncheck formats you don’t want sent to your e-book reader. You can also reorder the formats. The format at the top of the list (must be checked) will be the one used for automatic conversion when sending an e-book in an unsupported (or unchecked) format to the device.

### Task 6: The e-book viewer

I’ve hinted that calibre has the ability to view e-books too. All you need to do is select the e-book you want to read and click the ‘View’ button in the tool bar to have calibre open the e-book in calibre’s e-book viewer. The viewer supports everything you might expect such as bookmarks and navigation via the table of contents (if the e-book has one). The viewer, however, cannot read e-books protected with DRM.

## Where to get help

The first place to look for help is in the ‘Preferences’ dialog. All options have clear descriptions, and there are a lot of options. If you want to change something about calibre there may already be an option for it. It’s also a good idea to familiarize yourself with the preferences because parts of it, such as conversion, are just defaults and will be presented to you at different times for fine-tuning on a per e-book basis.

The next place to look is the [online user manual](https://manual.calibre-ebook.com). Click the ‘Help’ button in the tool bar to have the user manual open in your browser. There is a wealth of information in the user manual including tips and solutions to common problems. It’s also a good idea to check the calibre [FAQ](https://manual.calibre-ebook.com/faq.html) for answers to common questions.

Finally, there is the [calibre forum](https://www.mobileread.com/forums/forumdisplay.php?f=166) on [Mobileread](https://www.mobileread.com/) which is the official help forum. There are a number of knowledgeable users who answer questions. Also, Kovid and myself actively participate in helping new and veteran users. If you have a question or need help this is the best place to go. If you’ve found a bug or would like to request a new feature it’s okay to ask about it on the forum but it’s also a good idea to submit it to the projects [bug/issue tracking system](https://bugs.launchpad.net/calibre). Forum posts tend to get lost over time while the tracking system makes it easy to see what needs fixing or worked on.

