## REACT-DOM

`Là 1 thư viện là cầu nối giữa React và DOM`

`Sử dụng để render ReactElement ra trình duyệt`

`<script src="https://unpkg.com/react-dom@17/umd/react-dom.development.js" crossorigin></script>`

`Trước khi sử dụng thì phải add thẻ react vào`

`<script src="https://unpkg.com/react@17/umd/react.development.js" crossorigin></script>`

**`Thẻ React phải trước thẻ React-DOM nếu không sẽ gây lỗi`**

## Sử dụng

**`ReactDOM.render(element, container,callback)`**

```bash
      const divReact = React.createElement(
        "div",
        {
          className: "post-item",
        },
        React.createElement(
          "h2",
          {
            title: "Hoc React that la vui",
          },
          "Hoc ReactJS"
        ),
        React.createElement("p", null, "Hoc ReactJS tu co ban den nang cao")
      );

      // Get root element
      const root = document.getElementById("root");

      // React-DOM => render UI

      ReactDOM.render(divReact, root);
```
