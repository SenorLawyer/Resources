# Awesome Resources

A curated list of amazing resources for developers and designers.

## Table of Contents

- [Developer Tools](#developer-tools)
- [Studio Tools](#studio-tools)
- [Design Tools](#design-tools)
- [Web Development](#web-development)
- [Programming Languages](#programming-languages)
- [UI Libraries](#ui-libraries)
- [Learning and Tutorials](#learning-and-tutorials)
- [Networking](#networking)



## Developer Tools

- [Shodan](https://www.shodan.io/)
- [Automa](https://www.automa.site/)
- [PikaBackup](https://apps.gnome.org/en-GB/PikaBackup/)
- [Fish Shell](https://fishshell.com/)
- [Arch Linux Packages](https://archlinux.org/packages)
- [Paru AUR Helper](https://github.com/Morganamilo/paru)
- [Solaar](https://github.com/pwr-Solaar/Solaar)
- [Videomass](https://github.com/jeanslack/Videomass)
- [Trayer-srg](https://github.com/sargon/trayer-srg)
- [Vesktop](https://github.com/Vencord/Vesktop)

## Studio Tools
- [UIStrokeAdjuster](https://devforum.roblox.com/t/uistrokeadjuster-properly-scale-your-uistrokes/1889014)

## Design Tools

- [Gradient Magic](https://www.gradientmagic.com/)
- [Dribbble](https://dribbble.com/shots/popular)
- [Realtime Colors](https://www.realtimecolors.com/)
- [Figma](https://figma.com)
  - [React Icons Community File](https://www.figma.com/file/fEtbmW8gq2CTvxU5muuD2j/React-Icons-v4.3.1-(Community)?type=design&node-id=2-227&mode=design&t=CmMzvkiLHc3mb25V-0)
  - [Import React Icons Plugin](https://www.figma.com/community/plugin/921172243620367846/import-react-icons)
- [Mobbin](https://mobbin.com/browse/web/apps)

## Web Development

- [Build Your Own X](https://github.com/codecrafters-io/build-your-own-x)
- [Send](https://send.vis.ee)
- [The Stocks](https://v3.thestocks.im/)
- [Modified Mainte](https://github.com/AyoItsYas/Modified-Mainte?tab=readme-ov-file)
- [Dots Hyprland](https://github.com/end-4/dots-hyprland/tree/main?tab=readme-ov-file)
- [No Hello](https://nohello.net)
- [Eraser](https://app.eraser.io/)
- [React Three Fiber](https://docs.pmnd.rs/react-three-fiber/getting-started/introduction)
- [Downshift](https://www.downshift-js.com/)
- [CSS Grid Garden](https://cssgridgarden.com/)
- [Flexbox Froggy](https://flexboxfroggy.com/)
- [Centering a Div](https://www.joshwcomeau.com/css/center-a-div/)
- [Interactive Guide to Grid](https://www.joshwcomeau.com/css/interactive-guide-to-grid/)
- [Pandoc](https://pandoc.org/installing.html)
- [Recommended Screen Resolution for Web Design](https://thewhitelabelagency.com/recommended-screen-resolution-for-web-design/)
- [DaisyUI](https://daisyui.com/)
- [React Icons](https://react-icons.github.io/react-icons/)

## Programming Languages

- [Rust Book](https://doc.rust-lang.org/stable/book/)
- [Yew Tutorial](https://yew.rs/docs/next/tutorial)
- [Gpt4all](https://gpt4all.io/index.html)

## UI Libraries

- [Shadcn UI](https://ui.shadcn.com/)
- [React Aria](https://react-spectrum.adobe.com/react-aria/getting-started.html)
- [Radix UI](https://www.radix-ui.com/)
- [React Spectrum](https://react-spectrum.adobe.com/react-aria/getting-started.html)
- [MUI Core](https://mui.com/core/)
- [Aceternity UI](https://ui.aceternity.com/)

## Learning and Tutorials

- [React-Redux Audio Playing](https://stackoverflow.com/questions/42695145/how-to-handle-audio-playing-in-react-redux)
- [Controlling Scrollback Size in WezTerm](https://wezfurlong.org/wezterm/scrollback.html#controlling-the-scrollback-size)
- [Interactive Guide to Grid by Josh W. Comeau](https://www.joshwcomeau.com/css/interactive-guide-to-grid/)
- [React Spinners](https://www.davidhu.io/react-spinners/)

## Code Snippets

### Leave all groups
```js
import noblox from "noblox.js";

const cookie: string = "";
const userId: number = 1988525073;

async function LeaveGroups() {
  const currentUser = await noblox.setCookie(cookie);
  console.log(`Logged in as ${currentUser.UserName} [${currentUser.UserID}]`);

  let groups = await noblox.getGroups(userId);
  groups = groups.filter(
    (group) =>
      group.Id !== 17216028 &&
      group.Id !== 7586320 &&
      group.Id !== 7962297 &&
      group.Id !== 15774327 &&
      group.Id !== 32380007 &&
      group.Id !== 2627479 &&
      group.Id !== 2627480
  );

  await noblox.setCookie(cookie);

  while (groups.length > 0) {
    const group = groups.shift();
    console.log(`Leaving group ${group?.Name} [${group?.Id}]`);

    await noblox.leaveGroup(group!.Id);
  }
}

LeaveGroups();
```

## Networking

- [OPNSense](https://opnsense.org/)