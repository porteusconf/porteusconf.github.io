### Finding issues caused by updates
#### Windows first...
You can search at the "Windows release health dashboard" for your version (To find your version: start -> winver) For example [for win10-1909](https://docs.microsoft.com/en-us/windows/release-information/status-windows-10-1909)
It takes at least a few days for microsoft to admit to issues that show up first on reddit, askwoody.com, etc. Ask-woody maintains a MS-DEFCON rating of current dangerousness of patching at [https://www.askwoody.com/ms-defcon-system](https://www.askwoody.com/ms-defcon-system/)   Woody pretty well documents that for years Microsoft regularly issues faulty updates that, as a result of not having been thorougly tested, end up causing serious problems for more than a few folks. 

Here's a summary of the sad situation, especially for ordinary consumer of windows-home, of microsoft confusingly, constantly renaming release channels rather than better testing updates at [https://www.zdnet.com/article/microsoft-stop-feeding-bugs-to-a-billion-windows-10-users-heres-how/](https://www.zdnet.com/article/microsoft-stop-feeding-bugs-to-a-billion-windows-10-users-heres-how/) Two conclusions:
* Microsoft doesn’t test its mainstream patches on a wide enough variety of configurations, and
* Complaints made through official channels -- opened support cases, Feedback Hub, Microsoft Answers forum -- fall on deaf ears.

#### Apple updates also regularly cause issues that go unfixed for months (or forever!)
So, Mac users don't be smug... It is even harder to find known-issues let alone details for macos updates. And submitting bug reports is a opaque, difficult process as well. Un-managed macs (without MDM) can no longer turn off nagging notifications of major releases like 10.14 (mojave) to 10.15 (catalina). Details in links to [mrmackintosh.com at previous blog-post](https://porteusconf.github.io/2020/05/30/macos10.15-slow-by-design.html)

So for example, for macos-10.14 users, in a nutshell, starting with 2020-003 update to 10.14 apple is deprecating the ability for end-user to choose updates to ignore. Before 2020-003 you could turn off Apple naging you to update to 10.15, but after 2020-003 you can no longer turn off the nagging notificagtions. It is possible that "Starting with macOS 10.15.4, major releases of macOS can be deferred for up to 90 days using MDM.” This likely means the change was not backported to 10.14 and we will be unable to ignore 10.16 on Mojave." 
