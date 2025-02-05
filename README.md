<div align="center">
  <h1>
    Oh, hai! 🖖 I'm Jase.
  </h1>
  ~
  <p>
    I make stuff for the web using electricity 🔌 and an Apple 🍎💻.
  </p>
  <p>
    I'm guessing you can, too. 
  </p>
  <p>
    Which is pretty neat when you think about it. 🤯
  </p>
  <p>~</p>
  <p>
    Have a look at some of the things I've worked on...
  </p>
  <p>↯</p>
  &nbsp;
</div>

<h1>Proof of Work</h1>

<h2>NaviStats</h2>

  - A subscription-based web platform that provides reporting and tracking tools for companies in the real estate title industry. NaviStats is comprised of the two applications: TitleTrak and AgentMap.

    <h3>Challenges & Achievements</h3>

    - <h4>Customized Date Range Picker</h4>

      Builds upon Material UI's [Date Range Picker](https://mui.com/x/react-date-pickers/date-range-picker/#customize-the-field) component. Leverages the feature to easily select commonly used date ranges.

      https://github.com/user-attachments/assets/cd5e1ab3-04b1-4b5d-b295-8efc2c6bb807

    - The NaviStats marketing website ([navistats.com](https://navistats.com/)) is a WordPress site. The actual NaviStats web application, navistats.com/dashboard, is a React application served from the NaviStats WordPress site using the [ReactPress](https://wordpress.org/plugins/reactpress/) plugin.
      This required solutions for some unique issues created by the WordPress-React relationship. For example:

      <h4><b>Special route handling</b></h4>

        - WordPress handles URL routing by matching URL path segments to WordPress Pages. This includes routing users to the NaviStats Dashboard page (/dashboard) which loads the React application.
          But there's a limitation with the Dashboard's ability to handle routing operations using a tool like `react-router`.

          For example, if I wanted to show in the user's URL that AgentMap is currenlty loaded, I ideally would like the URL to read as navistats.com/dashboard/agent-map. However, this will not work as intended. The WordPress router will attempt to load a WP Page that's assigned to the /agent-map route, which doesn't exist. React will never get the chance to load and control the routing to the React-based AgentMap and TitleTrak applications.

          In order to allow some kind of URL customization that represented a user's current application and application state, I decided to leverage the search parameter component of a URL. 

      <h4><b>WordPress Metadata API for simple data storage</b></h4>

      <h4><b>Instrusive UI when logged in as WordPress admin</b></h4>

      <h4><b>No option for server-side rendering</b></h4>

&nbsp;

<h2>MetaMask</h2>

<details open>
  <summary>Open-Source Contributions</summary>
  
  &nbsp;
  - [#20701](https://github.com/MetaMask/metamask-extension/pull/20701)
    - Issue: `<ConfirmationNetworkSwitch/>` contains deprecated components.
    - Solution: Replace `<Box/>`, `<Typography/>`, & `<SiteIcon/>` with counterparts from `component-library`.
    - [Discovered reason for failed attempts at updating UI snapshots for Jest tests.](https://github.com/MetaMask/metamask-extension/pull/20701#issuecomment-1744033518)
  
  - [#20579](https://github.com/MetaMask/metamask-extension/pull/20579)
    - Issue: `<Chip/>` has been deprecated in favor of `<Tag/>`.
    - Solution: Add deprecation warnings for `<Chip/>` to its JSDocs and Storybook.
  
  - [#20432](https://github.com/MetaMask/metamask-extension/pull/20432)
    - Issue: 'Decrypt Request' view only shows part of a long decrypted message.
    - Solution: Allow the decryted message box to be scrollable.
  
  - [#19944](https://github.com/MetaMask/metamask-extension/pull/19944)
    - Issue: Misaligned icons in 'Connected Sites' dropdown menu.
    - Solution: Replaced a deprecated UI component with newer shared component.
    - [Helped another contributor get started on their first issue.](https://github.com/MetaMask/metamask-extension/issues/19901#issuecomment-1631045017)
</details>

&nbsp;

<h2>Carvana</h2>

  - In Carvana's income verification flow, a user is expected to upload proof of income documention. I implemented the UI/UX responsible for capturing those documents. ([Demo](https://github.com/jase-b/carvana-ui-demo#in-carvanas-income-verification-flow-a-user-is-expected-to-upload-proof-of-income-documention-i-implemented-the-uiux-currently-used-to-capture-those-documents-see-the-code) | [Code](https://github.com/jase-b/carvana-ui-demo/tree/main/pay-stub-upload))
  
  - I implemented the newer, simpler design for the driver's license upload experience. ([Demo](https://github.com/jase-b/carvana-ui-demo/tree/main/drivers-license-upload#carvana-ui-demo) | [Code](https://github.com/jase-b/carvana-ui-demo/tree/main/drivers-license-upload))

&nbsp;

<h2>Nice Credenza</h2>

  - Nice Credenza was a Shopify store that sold credenzas, sideboards, buffets, and other storage-like home furnishings.

  - I designed and implemented the About page. ([Design](https://github.com/jase-b/nice-credenza#design-for-about-page) | [Code](https://github.com/jase-b/nice-credenza/tree/master))
