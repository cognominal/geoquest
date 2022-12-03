## Geoquest quests, their modes and their URLs

Note: this is an informal specification. Everything has not been yet
implemented.

Geoquest can run different quests in different modes for different parts of the
world. Each quest has its own
[URL](https://www.geeksforgeeks.org/components-of-a-url/) that you can share.
Unrecognized parts of an URL query string are silently ignored. Thru the menu,
you can access the daily quest.


Initially you are presented with a map of the world. Hovering or clicking
allows to transitively search a part of the world and select it for a quest. 
As you search further, you zoom in zones with further granularity. 

Once you have found a quest that suits you, okay it to start that specific
quest. For example you can choose Europe, then Western Europe and than German
Landers. If you zoom out, if you have not selected your quest, you get back to
a proposed quest on a larger area. You can use the menu to adjust the quest
mode. That will restart the quest. The mode dictates the infos that will be
presented for searching the zone. That can be a combination of name, flag or
other specific informations if available for the zone choosen for the quest.

## Saving you achievements

On a given browser, the state of your progress is maintained.
Thru the menu you can see the list of propoosed achievments.
Eventually you shoud be able to cut and paste the states from
one browser to another.

## Proposing newer quests

You can create quests for specific part of the world 
by adding and  editiong appropriate json and geogjson file

You can share them with [pull
requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)

## Developing

You can use whatever editor but [vscode](https://code.visualstudio.com/) makes life easier.

## Developping within a browser 

You can ever edit and run geoquest from within chrome or firefox
using [codespaces](https://devblogs.microsoft.com/visualstudio/introducing-visual-studio-codespaces/). Doing so will use a
managed [container](https://containers.dev/) and will free you from installing anything on your computer.

Assuming you already have a github account. Just open [Geoquest github
repo](https://github.com/woutdp/geoquest), type '.' in the window and you get a
vscode editor on the page. Click on the button on the lower left, you get a
menu, pick "Continue working on", then pick "Create new code space". After a
few more steps you got a running container. You can have share the container
URL to team work.

## Geoquest as a vscode extension

Support of Geoquest as a vscode extension is a possibility too
that would allow to use Geoquest without Net connectivity.

## Developping

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server.
Note if you develop the project in a container, the npm install 
has been done when starting the container.

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open

# to automatically format the code
npm run format
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

## Contributing

The code at the moment is still a bit messy, especially the code for handling different 'game modes'. Feel free to refactor, fix or add features.
