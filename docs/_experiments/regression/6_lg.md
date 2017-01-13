---
layout: fullscreen_graph
---

<html lang="en" id="report-container">
    <head>
        <meta charset="utf-8">
        <title>Bayesian Regression</title>
        
<link rel="stylesheet" href="https://cdn.pydata.org/bokeh/release/bokeh-0.12.3.min.css" type="text/css" />
        
<script type="text/javascript" src="https://cdn.pydata.org/bokeh/release/bokeh-0.12.3.min.js"></script>
<script type="text/javascript">
    Bokeh.set_log_level("info");
</script>
        <style>
          html {
            width: 100%;
            height: 100%;
          }
          body {
            width: 90%;
            height: 100%;
            margin: auto;
          }
        </style>
    </head>
    <body>
        
        <div class="bk-root">
            <div class="plotdiv" id="c3f3106e-f28c-4c18-b27d-cf0f4bbacda8"></div>
        </div>
        
        <script type="text/javascript">
            Bokeh.$(function() {
            Bokeh.safely(function() {
                var docs_json = {"ecfea1dd-721d-4714-b7c7-a3cda7b2ac8f":{"roots":{"references":[{"attributes":{"callback":null,"overlay":{"id":"9a65a03d-fd49-4d09-811e-f135d3329149","type":"BoxAnnotation"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"renderers":[{"id":"5ce8166d-bfe8-4b1d-a963-e762594d078b","type":"GlyphRenderer"},{"id":"b158ae26-6eda-48e3-b48a-940fcdb7ca94","type":"GlyphRenderer"}]},"id":"2c0a7df9-bbf1-45b1-a544-8d36d609e929","type":"BoxSelectTool"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":12},"x_start":{"value":12},"y_end":{"value":0.0},"y_start":{"value":0.7422573903987334}},"id":"e88945f9-9ea8-4fe7-a254-95b85a11ec48","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":29},"x_start":{"value":29},"y_end":{"value":0.75},"y_start":{"value":0.13721175181824818}},"id":"b91bf867-9871-4e8d-b44c-499c87f2e655","type":"Arrow"},{"attributes":{"bottom_units":"screen","fill_alpha":{"value":0.5},"fill_color":{"value":"lightgrey"},"left_units":"screen","level":"overlay","line_alpha":{"value":1.0},"line_color":{"value":"black"},"line_dash":[4,4],"line_width":{"value":2},"plot":null,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"9a65a03d-fd49-4d09-811e-f135d3329149","type":"BoxAnnotation"},{"attributes":{},"id":"63de8988-e7cb-48fb-ba4f-14196526387c","type":"BasicTickFormatter"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":53},"x_start":{"value":53},"y_end":{"value":0.0},"y_start":{"value":0.7422573903987334}},"id":"898a5db8-bf1d-465c-9732-38887a41b3eb","type":"Arrow"},{"attributes":{"items":[{"id":"95548d21-fa94-4239-81be-50b46dfc2b2d","type":"LegendItem"},{"id":"5273a503-1245-48d8-9ee1-a85de90afef5","type":"LegendItem"}],"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"}},"id":"5a661108-ff8f-4af0-ba2e-f70ee8e78e04","type":"Legend"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":16},"x_start":{"value":16},"y_end":{"value":0.6},"y_start":{"value":0.8359380739869442}},"id":"e1a04f0f-c88c-461c-a4a0-02f4a052708f","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":39},"x_start":{"value":39},"y_end":{"value":0.9},"y_start":{"value":1.0814854881631526}},"id":"75f86577-34bc-4e48-848d-1d6914cccd7b","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":36},"x_start":{"value":36},"y_end":{"value":0.8},"y_start":{"value":1.321040482893281}},"id":"c38475ae-9a59-4c55-a3b5-e1efb4e727a3","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":18},"x_start":{"value":18},"y_end":{"value":0.75},"y_start":{"value":0.7102073181250088}},"id":"f37cc522-078b-4c44-8fe3-66894c0840c7","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":10},"x_start":{"value":10},"y_end":{"value":1.0},"y_start":{"value":0.857675070012604}},"id":"4d284268-5be2-4cfe-84de-38e174feaa85","type":"Arrow"},{"attributes":{"data_source":{"id":"0e1c9bb2-7347-4185-8791-b56c94107e2f","type":"ColumnDataSource"},"glyph":{"id":"d1b772e7-f78d-4813-8317-c4969cf95fea","type":"Square"},"hover_glyph":null,"nonselection_glyph":{"id":"7cc5e8e6-c374-4cc9-aa92-73790f98bddf","type":"Square"},"selection_glyph":null},"id":"5ce8166d-bfe8-4b1d-a963-e762594d078b","type":"GlyphRenderer"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":11},"x_start":{"value":11},"y_end":{"value":0.55},"y_start":{"value":0.6683145989573528}},"id":"8e0ab863-57ae-4c44-985f-5658470894c0","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":47},"x_start":{"value":47},"y_end":{"value":0.55},"y_start":{"value":0.7999503848163277}},"id":"fcd59ae8-697c-4422-ae44-f44e189a962c","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":52},"x_start":{"value":52},"y_end":{"value":0.7},"y_start":{"value":1.0950355690018458}},"id":"3e71fa41-335a-4fd8-9870-66a71ccedf2f","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":41},"x_start":{"value":41},"y_end":{"value":0.85},"y_start":{"value":0.7575222541658843}},"id":"e58e378a-6ff1-4294-88f3-b89168cf369d","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":46},"x_start":{"value":46},"y_end":{"value":0.9},"y_start":{"value":0.41374093532096023}},"id":"2cac0ba2-0d02-43a3-b2ed-0b914172b54c","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":17},"x_start":{"value":17},"y_end":{"value":0.8},"y_start":{"value":0.8397908298742917}},"id":"0478d32a-575f-491f-99d3-9e1fc14b03f6","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":31},"x_start":{"value":31},"y_end":{"value":0.9},"y_start":{"value":0.44131550765753425}},"id":"83c6300e-9d97-4cc5-9873-a192824c0121","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":50},"x_start":{"value":50},"y_end":{"value":0.7},"y_start":{"value":1.3996636278329615}},"id":"ba66d80a-216b-44d7-8cb0-a32953f3fd1b","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":54},"x_start":{"value":54},"y_end":{"value":0.6},"y_start":{"value":0.5511947188936891}},"id":"52599cc0-84e8-413a-9e27-853dc705c8e1","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":20},"x_start":{"value":20},"y_end":{"value":0.6},"y_start":{"value":0.7508897332266687}},"id":"7b76318f-d034-401f-a1f1-7da1a5b3efeb","type":"Arrow"},{"attributes":{"below":[{"id":"1cc09dcd-4337-4a6b-8a21-ed7aea34d4eb","type":"LinearAxis"}],"left":[{"id":"8725351e-d6aa-4a8c-a076-279691d7b5b6","type":"LinearAxis"}],"plot_height":700,"plot_width":1020,"renderers":[{"id":"1cc09dcd-4337-4a6b-8a21-ed7aea34d4eb","type":"LinearAxis"},{"id":"dbe08ab0-8103-4a43-95c7-3bbf14f7521f","type":"Grid"},{"id":"8725351e-d6aa-4a8c-a076-279691d7b5b6","type":"LinearAxis"},{"id":"a171ebef-88b3-4999-a19a-d814d84eead6","type":"Grid"},{"id":"4ae2eb6f-2e14-4345-894f-dc0259a109e1","type":"BoxAnnotation"},{"id":"9a65a03d-fd49-4d09-811e-f135d3329149","type":"BoxAnnotation"},{"id":"12b71738-746d-41ad-afd8-2bb534c23973","type":"Arrow"},{"id":"ee0e41bd-6fe1-49a2-92a9-fd79a501b428","type":"Arrow"},{"id":"ec59180e-1b9f-420e-86e6-59e06bc6f641","type":"Arrow"},{"id":"b32b6f24-4865-4c4e-86b0-4c8e1218c53d","type":"Arrow"},{"id":"bdf46b22-6b09-4040-b152-3dc1f1f9aa7b","type":"Arrow"},{"id":"90dc3e5a-c471-49d1-98ea-ebd3717e577f","type":"Arrow"},{"id":"45a27a5b-792c-4e08-aeff-142b9895aacd","type":"Arrow"},{"id":"6e84d2c5-71bc-4039-a919-e6d1043acaf6","type":"Arrow"},{"id":"ee91aa0b-9f63-4e24-b974-7d8b3241e5bb","type":"Arrow"},{"id":"790615e0-613f-4cb1-82db-d694a2d63fbf","type":"Arrow"},{"id":"4d284268-5be2-4cfe-84de-38e174feaa85","type":"Arrow"},{"id":"8e0ab863-57ae-4c44-985f-5658470894c0","type":"Arrow"},{"id":"e88945f9-9ea8-4fe7-a254-95b85a11ec48","type":"Arrow"},{"id":"5566c113-749e-49aa-8e35-d5d9748ca1b2","type":"Arrow"},{"id":"37a8cd8f-2f16-4789-9e08-dd571de02735","type":"Arrow"},{"id":"ab0d37c4-8a98-475e-be20-cc57adcdd459","type":"Arrow"},{"id":"e1a04f0f-c88c-461c-a4a0-02f4a052708f","type":"Arrow"},{"id":"0478d32a-575f-491f-99d3-9e1fc14b03f6","type":"Arrow"},{"id":"f37cc522-078b-4c44-8fe3-66894c0840c7","type":"Arrow"},{"id":"2bcf9c6b-3fa0-428a-b1e7-902d05ba7c2c","type":"Arrow"},{"id":"7b76318f-d034-401f-a1f1-7da1a5b3efeb","type":"Arrow"},{"id":"3cce78eb-a50c-4723-9f5f-e5d730dd8387","type":"Arrow"},{"id":"d845eef7-d526-4b06-a2da-a2e2baeade66","type":"Arrow"},{"id":"db9b532c-d54a-4dd3-9f1b-312837fdffc1","type":"Arrow"},{"id":"b36740c5-dcc3-4cc5-a541-312888f35b0b","type":"Arrow"},{"id":"52675a56-a887-4d50-b372-060c4d4c91e7","type":"Arrow"},{"id":"81311aad-b0f7-460f-b736-9f6f6ce492f9","type":"Arrow"},{"id":"e29d47e7-edf0-43a4-b059-40077522e77c","type":"Arrow"},{"id":"3109eb6e-d63b-4519-8c0b-b7bd22351c74","type":"Arrow"},{"id":"b91bf867-9871-4e8d-b44c-499c87f2e655","type":"Arrow"},{"id":"dd3cbf65-064e-4f61-9e6a-931354321897","type":"Arrow"},{"id":"83c6300e-9d97-4cc5-9873-a192824c0121","type":"Arrow"},{"id":"4b515852-2a6b-419b-a9fb-cbc920dfdcf6","type":"Arrow"},{"id":"1c1fbfd8-dcd2-48e9-9852-de8be613921c","type":"Arrow"},{"id":"698c991d-8ced-4e08-92a1-2ed08334bfd7","type":"Arrow"},{"id":"f3f723f0-0aca-4a74-aaa3-259cf13f9b22","type":"Arrow"},{"id":"c38475ae-9a59-4c55-a3b5-e1efb4e727a3","type":"Arrow"},{"id":"ebd2e6a0-8341-4222-9343-43e06f616b72","type":"Arrow"},{"id":"3cccaf54-2846-48dd-9ebc-24a0f1679284","type":"Arrow"},{"id":"75f86577-34bc-4e48-848d-1d6914cccd7b","type":"Arrow"},{"id":"f3dcd172-9a35-4568-a38f-572142b1cbee","type":"Arrow"},{"id":"e58e378a-6ff1-4294-88f3-b89168cf369d","type":"Arrow"},{"id":"8f4c87b8-a93e-4252-9d01-3a53affdba25","type":"Arrow"},{"id":"97781c29-e9f9-45c8-8a7f-428c43b725be","type":"Arrow"},{"id":"77d2eeda-ca1d-452b-8a87-3043a96d69bd","type":"Arrow"},{"id":"81042c70-85f7-4310-bbb8-24137f7aeed2","type":"Arrow"},{"id":"2cac0ba2-0d02-43a3-b2ed-0b914172b54c","type":"Arrow"},{"id":"fcd59ae8-697c-4422-ae44-f44e189a962c","type":"Arrow"},{"id":"17d56545-f30a-4746-9c35-b745ac0b7e93","type":"Arrow"},{"id":"c5692d2f-a53b-4b41-b71d-026a2ed32b6c","type":"Arrow"},{"id":"ba66d80a-216b-44d7-8cb0-a32953f3fd1b","type":"Arrow"},{"id":"21754add-95ff-4111-ac6c-65a8a632aaf3","type":"Arrow"},{"id":"3e71fa41-335a-4fd8-9870-66a71ccedf2f","type":"Arrow"},{"id":"898a5db8-bf1d-465c-9732-38887a41b3eb","type":"Arrow"},{"id":"52599cc0-84e8-413a-9e27-853dc705c8e1","type":"Arrow"},{"id":"fd0725c3-401c-4dcc-96e6-369a8a256b49","type":"Arrow"},{"id":"91cd5fe3-03a5-49da-8504-0d5e90f2b319","type":"Arrow"},{"id":"502e2d0d-3616-40e7-8c40-1b6058ece1a9","type":"Arrow"},{"id":"56736cdc-5667-4a20-b3e8-3c01491ecf62","type":"Arrow"},{"id":"96f0e298-d550-4b46-922f-a4ed992d768a","type":"Arrow"},{"id":"1204bfb0-a3a3-424a-b3be-7f26bec3380d","type":"Arrow"},{"id":"554e6fff-ab2c-453c-bcba-5a3a0ee817b0","type":"Arrow"},{"id":"3b910486-02df-4710-8c60-625d7782207c","type":"Arrow"},{"id":"d3e4ad73-5afd-44d5-870a-30c1d05fc469","type":"Arrow"},{"id":"b370ab80-80b5-4a50-9588-2a548e2cc2fd","type":"Arrow"},{"id":"5a661108-ff8f-4af0-ba2e-f70ee8e78e04","type":"Legend"},{"id":"5ce8166d-bfe8-4b1d-a963-e762594d078b","type":"GlyphRenderer"},{"id":"b158ae26-6eda-48e3-b48a-940fcdb7ca94","type":"GlyphRenderer"}],"title":{"id":"d989ae00-73fa-4f08-82ba-d99fdabab30f","type":"Title"},"tool_events":{"id":"9d5b22ac-9d0b-40af-8bd3-1fdacbe00ca3","type":"ToolEvents"},"toolbar":{"id":"34a3fbdd-fb42-4643-817b-60bfd39a9f7c","type":"Toolbar"},"x_range":{"id":"bdc37559-c241-40aa-b250-942e3bc2c14c","type":"DataRange1d"},"y_range":{"id":"132f91c2-e427-44ea-acdb-789c73d8cc5c","type":"DataRange1d"}},"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":26},"x_start":{"value":26},"y_end":{"value":0.63},"y_start":{"value":0.7938618356842688}},"id":"81311aad-b0f7-460f-b736-9f6f6ce492f9","type":"Arrow"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"x":{"field":"x"},"y":{"field":"y"}},"id":"ffd616a7-ee66-4e1d-8597-2b081529ca20","type":"Circle"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":45},"x_start":{"value":45},"y_end":{"value":0.0},"y_start":{"value":0.7422573903987334}},"id":"81042c70-85f7-4310-bbb8-24137f7aeed2","type":"Arrow"},{"attributes":{"fill_alpha":{"value":0.3},"fill_color":{"value":"blue"},"line_alpha":{"value":0.3},"line_color":{"value":"blue"},"x":{"field":"x"},"y":{"field":"y"}},"id":"0dc77476-ac0d-48d7-a890-81fdddf14390","type":"Circle"},{"attributes":{"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"}},"id":"fda3f114-a914-4f70-916b-d6eb1cd0ae40","type":"PanTool"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":33},"x_start":{"value":33},"y_end":{"value":1.0},"y_start":{"value":0.7110039036513138}},"id":"1c1fbfd8-dcd2-48e9-9852-de8be613921c","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":13},"x_start":{"value":13},"y_end":{"value":0.65},"y_start":{"value":0.6618415450946266}},"id":"5566c113-749e-49aa-8e35-d5d9748ca1b2","type":"Arrow"},{"attributes":{},"id":"d25072ea-a7ef-4ca1-9bf4-fe2d0eb72b2a","type":"BasicTickFormatter"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":2},"x_start":{"value":2},"y_end":{"value":0.9},"y_start":{"value":0.891589912937713}},"id":"ec59180e-1b9f-420e-86e6-59e06bc6f641","type":"Arrow"},{"attributes":{"callback":null,"column_names":["y","x"],"data":{"x":[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64],"y":[0.8,0.85,0.9,0.7,0.9,0.8,0.9,0.75,0.8,0.7,1.0,0.55,0.0,0.65,1.0,0.7,0.6,0.8,0.75,0.6,0.6,0.9,0.0,0.85,0.75,0.0,0.63,0.9,0.65,0.75,0.8,0.9,0.0,1.0,0.0,1.0,0.8,0.8,0.8,0.9,0.8,0.85,0.6,0.55,0.8,0.0,0.9,0.55,0.0,0.85,0.7,0.55,0.7,0.0,0.6,0.9,0.6,0.9,0.8,0.9,0.95,1.0,0.0,0.9,0.9]}},"id":"f305c008-3dd9-4cbc-896d-5296dc60c86f","type":"ColumnDataSource"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":19},"x_start":{"value":19},"y_end":{"value":0.6},"y_start":{"value":0.758158707833525}},"id":"2bcf9c6b-3fa0-428a-b1e7-902d05ba7c2c","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":9},"x_start":{"value":9},"y_end":{"value":0.7},"y_start":{"value":0.35052509222378814}},"id":"790615e0-613f-4cb1-82db-d694a2d63fbf","type":"Arrow"},{"attributes":{"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"ticker":{"id":"c635ece1-2829-4106-acf7-7681397426bf","type":"BasicTicker"}},"id":"dbe08ab0-8103-4a43-95c7-3bbf14f7521f","type":"Grid"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":3},"x_start":{"value":3},"y_end":{"value":0.7},"y_start":{"value":0.5631736337050302}},"id":"b32b6f24-4865-4c4e-86b0-4c8e1218c53d","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":0},"x_start":{"value":0},"y_end":{"value":0.8},"y_start":{"value":0.9609553856206925}},"id":"12b71738-746d-41ad-afd8-2bb534c23973","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":8},"x_start":{"value":8},"y_end":{"value":0.8},"y_start":{"value":0.7560258293373403}},"id":"ee91aa0b-9f63-4e24-b974-7d8b3241e5bb","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":44},"x_start":{"value":44},"y_end":{"value":0.8},"y_start":{"value":0.1950196927352178}},"id":"77d2eeda-ca1d-452b-8a87-3043a96d69bd","type":"Arrow"},{"attributes":{"data_source":{"id":"f305c008-3dd9-4cbc-896d-5296dc60c86f","type":"ColumnDataSource"},"glyph":{"id":"0dc77476-ac0d-48d7-a890-81fdddf14390","type":"Circle"},"hover_glyph":null,"nonselection_glyph":{"id":"ffd616a7-ee66-4e1d-8597-2b081529ca20","type":"Circle"},"selection_glyph":null},"id":"b158ae26-6eda-48e3-b48a-940fcdb7ca94","type":"GlyphRenderer"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":25},"x_start":{"value":25},"y_end":{"value":0.0},"y_start":{"value":0.7422573903987334}},"id":"52675a56-a887-4d50-b372-060c4d4c91e7","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":7},"x_start":{"value":7},"y_end":{"value":0.75},"y_start":{"value":0.608510097304919}},"id":"6e84d2c5-71bc-4039-a919-e6d1043acaf6","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":21},"x_start":{"value":21},"y_end":{"value":0.9},"y_start":{"value":1.0630161270610579}},"id":"3cce78eb-a50c-4723-9f5f-e5d730dd8387","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":42},"x_start":{"value":42},"y_end":{"value":0.6},"y_start":{"value":1.0207596071143321}},"id":"8f4c87b8-a93e-4252-9d01-3a53affdba25","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":28},"x_start":{"value":28},"y_end":{"value":0.65},"y_start":{"value":0.828753322704563}},"id":"3109eb6e-d63b-4519-8c0b-b7bd22351c74","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":58},"x_start":{"value":58},"y_end":{"value":0.8},"y_start":{"value":0.6977601748240224}},"id":"56736cdc-5667-4a20-b3e8-3c01491ecf62","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":24},"x_start":{"value":24},"y_end":{"value":0.75},"y_start":{"value":0.9805578228005196}},"id":"b36740c5-dcc3-4cc5-a541-312888f35b0b","type":"Arrow"},{"attributes":{"active_drag":"auto","active_scroll":"auto","active_tap":"auto","tools":[{"id":"fda3f114-a914-4f70-916b-d6eb1cd0ae40","type":"PanTool"},{"id":"8670558d-e0ac-4580-88ea-3d9c21945123","type":"WheelZoomTool"},{"id":"6d261766-7031-45f0-9df6-5acc049c403e","type":"BoxZoomTool"},{"id":"b37d2ca8-ff75-4ce5-a259-fed1bf4c8172","type":"ResetTool"},{"id":"b8f01fbc-7145-4e2e-8500-fe7dd5d08650","type":"SaveTool"},{"id":"2c0a7df9-bbf1-45b1-a544-8d36d609e929","type":"BoxSelectTool"}]},"id":"34a3fbdd-fb42-4643-817b-60bfd39a9f7c","type":"Toolbar"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":4},"x_start":{"value":4},"y_end":{"value":0.9},"y_start":{"value":0.572122085772931}},"id":"bdf46b22-6b09-4040-b152-3dc1f1f9aa7b","type":"Arrow"},{"attributes":{"callback":null,"column_names":["y","x"],"data":{"x":[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64],"y":[0.9609553856206925,0.20484760725676343,0.891589912937713,0.5631736337050302,0.572122085772931,0.8546624017675263,1.0039170122010679,0.608510097304919,0.7560258293373403,0.35052509222378814,0.857675070012604,0.6683145989573528,0.7422573903987334,0.6618415450946266,0.4740051950638078,1.7338533314322264,0.8359380739869442,0.8397908298742917,0.7102073181250088,0.758158707833525,0.7508897332266687,1.0630161270610579,0.7422573903987334,0.704560872313009,0.9805578228005196,0.7422573903987334,0.7938618356842688,0.44316527518209436,0.828753322704563,0.13721175181824818,0.5410630867697698,0.44131550765753425,0.7422573903987334,0.7110039036513138,0.7422573903987334,0.3614193966909928,1.321040482893281,0.6859679153045011,0.9054791880442197,1.0814854881631526,0.763767884765485,0.7575222541658843,1.0207596071143321,0.8580427025261346,0.1950196927352178,0.7422573903987334,0.41374093532096023,0.7999503848163277,0.7422573903987334,0.6112175327864833,1.3996636278329615,0.7321995654974084,1.0950355690018458,0.7422573903987334,0.5511947188936891,0.9540063546072358,0.4723693594443411,0.8900705210033266,0.6977601748240224,0.5849777036448012,1.127284550147693,0.901859664969989,0.7422112686177654,0.8031620987555914,1.4359098625687667]}},"id":"0e1c9bb2-7347-4185-8791-b56c94107e2f","type":"ColumnDataSource"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":22},"x_start":{"value":22},"y_end":{"value":0.0},"y_start":{"value":0.7422573903987334}},"id":"d845eef7-d526-4b06-a2da-a2e2baeade66","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":23},"x_start":{"value":23},"y_end":{"value":0.85},"y_start":{"value":0.704560872313009}},"id":"db9b532c-d54a-4dd3-9f1b-312837fdffc1","type":"Arrow"},{"attributes":{"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"}},"id":"8670558d-e0ac-4580-88ea-3d9c21945123","type":"WheelZoomTool"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":15},"x_start":{"value":15},"y_end":{"value":0.7},"y_start":{"value":1.7338533314322264}},"id":"ab0d37c4-8a98-475e-be20-cc57adcdd459","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":27},"x_start":{"value":27},"y_end":{"value":0.9},"y_start":{"value":0.44316527518209436}},"id":"e29d47e7-edf0-43a4-b059-40077522e77c","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":60},"x_start":{"value":60},"y_end":{"value":0.95},"y_start":{"value":1.127284550147693}},"id":"1204bfb0-a3a3-424a-b3be-7f26bec3380d","type":"Arrow"},{"attributes":{"label":{"value":"Predicted"},"renderers":[{"id":"5ce8166d-bfe8-4b1d-a963-e762594d078b","type":"GlyphRenderer"}]},"id":"95548d21-fa94-4239-81be-50b46dfc2b2d","type":"LegendItem"},{"attributes":{"plot":null,"text":"Bayesian Regression"},"id":"d989ae00-73fa-4f08-82ba-d99fdabab30f","type":"Title"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":5},"x_start":{"value":5},"y_end":{"value":0.8},"y_start":{"value":0.8546624017675263}},"id":"90dc3e5a-c471-49d1-98ea-ebd3717e577f","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":48},"x_start":{"value":48},"y_end":{"value":0.0},"y_start":{"value":0.7422573903987334}},"id":"17d56545-f30a-4746-9c35-b745ac0b7e93","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":1},"x_start":{"value":1},"y_end":{"value":0.85},"y_start":{"value":0.20484760725676343}},"id":"ee0e41bd-6fe1-49a2-92a9-fd79a501b428","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":30},"x_start":{"value":30},"y_end":{"value":0.8},"y_start":{"value":0.5410630867697698}},"id":"dd3cbf65-064e-4f61-9e6a-931354321897","type":"Arrow"},{"attributes":{"callback":null},"id":"bdc37559-c241-40aa-b250-942e3bc2c14c","type":"DataRange1d"},{"attributes":{"callback":null},"id":"132f91c2-e427-44ea-acdb-789c73d8cc5c","type":"DataRange1d"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":6},"x_start":{"value":6},"y_end":{"value":0.9},"y_start":{"value":1.0039170122010679}},"id":"45a27a5b-792c-4e08-aeff-142b9895aacd","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":64},"x_start":{"value":64},"y_end":{"value":0.9},"y_start":{"value":1.4359098625687667}},"id":"b370ab80-80b5-4a50-9588-2a548e2cc2fd","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":34},"x_start":{"value":34},"y_end":{"value":0.0},"y_start":{"value":0.7422573903987334}},"id":"698c991d-8ced-4e08-92a1-2ed08334bfd7","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":57},"x_start":{"value":57},"y_end":{"value":0.9},"y_start":{"value":0.8900705210033266}},"id":"502e2d0d-3616-40e7-8c40-1b6058ece1a9","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":14},"x_start":{"value":14},"y_end":{"value":1.0},"y_start":{"value":0.4740051950638078}},"id":"37a8cd8f-2f16-4789-9e08-dd571de02735","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":40},"x_start":{"value":40},"y_end":{"value":0.8},"y_start":{"value":0.763767884765485}},"id":"f3dcd172-9a35-4568-a38f-572142b1cbee","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":37},"x_start":{"value":37},"y_end":{"value":0.8},"y_start":{"value":0.6859679153045011}},"id":"ebd2e6a0-8341-4222-9343-43e06f616b72","type":"Arrow"},{"attributes":{"label":{"value":"Actual"},"renderers":[{"id":"b158ae26-6eda-48e3-b48a-940fcdb7ca94","type":"GlyphRenderer"}]},"id":"5273a503-1245-48d8-9ee1-a85de90afef5","type":"LegendItem"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":56},"x_start":{"value":56},"y_end":{"value":0.6},"y_start":{"value":0.4723693594443411}},"id":"91cd5fe3-03a5-49da-8504-0d5e90f2b319","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":35},"x_start":{"value":35},"y_end":{"value":1.0},"y_start":{"value":0.3614193966909928}},"id":"f3f723f0-0aca-4a74-aaa3-259cf13f9b22","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":51},"x_start":{"value":51},"y_end":{"value":0.55},"y_start":{"value":0.7321995654974084}},"id":"21754add-95ff-4111-ac6c-65a8a632aaf3","type":"Arrow"},{"attributes":{"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"}},"id":"b37d2ca8-ff75-4ce5-a259-fed1bf4c8172","type":"ResetTool"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":62},"x_start":{"value":62},"y_end":{"value":0.0},"y_start":{"value":0.7422112686177654}},"id":"3b910486-02df-4710-8c60-625d7782207c","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":63},"x_start":{"value":63},"y_end":{"value":0.9},"y_start":{"value":0.8031620987555914}},"id":"d3e4ad73-5afd-44d5-870a-30c1d05fc469","type":"Arrow"},{"attributes":{"dimension":1,"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"ticker":{"id":"854c8e62-310d-48b1-94eb-f5e915c89a8c","type":"BasicTicker"}},"id":"a171ebef-88b3-4999-a19a-d814d84eead6","type":"Grid"},{"attributes":{},"id":"c635ece1-2829-4106-acf7-7681397426bf","type":"BasicTicker"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":55},"x_start":{"value":55},"y_end":{"value":0.9},"y_start":{"value":0.9540063546072358}},"id":"fd0725c3-401c-4dcc-96e6-369a8a256b49","type":"Arrow"},{"attributes":{},"id":"854c8e62-310d-48b1-94eb-f5e915c89a8c","type":"BasicTicker"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":43},"x_start":{"value":43},"y_end":{"value":0.55},"y_start":{"value":0.8580427025261346}},"id":"97781c29-e9f9-45c8-8a7f-428c43b725be","type":"Arrow"},{"attributes":{"fill_alpha":{"value":0.5},"fill_color":{"value":"red"},"line_alpha":{"value":0.5},"line_color":{"value":"red"},"x":{"field":"x"},"y":{"field":"y"}},"id":"d1b772e7-f78d-4813-8317-c4969cf95fea","type":"Square"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":49},"x_start":{"value":49},"y_end":{"value":0.85},"y_start":{"value":0.6112175327864833}},"id":"c5692d2f-a53b-4b41-b71d-026a2ed32b6c","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":61},"x_start":{"value":61},"y_end":{"value":1.0},"y_start":{"value":0.901859664969989}},"id":"554e6fff-ab2c-453c-bcba-5a3a0ee817b0","type":"Arrow"},{"attributes":{"overlay":{"id":"4ae2eb6f-2e14-4345-894f-dc0259a109e1","type":"BoxAnnotation"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"}},"id":"6d261766-7031-45f0-9df6-5acc049c403e","type":"BoxZoomTool"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"x":{"field":"x"},"y":{"field":"y"}},"id":"7cc5e8e6-c374-4cc9-aa92-73790f98bddf","type":"Square"},{"attributes":{"axis_label":"test sqwaks","formatter":{"id":"63de8988-e7cb-48fb-ba4f-14196526387c","type":"BasicTickFormatter"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"ticker":{"id":"c635ece1-2829-4106-acf7-7681397426bf","type":"BasicTicker"}},"id":"1cc09dcd-4337-4a6b-8a21-ed7aea34d4eb","type":"LinearAxis"},{"attributes":{},"id":"9d5b22ac-9d0b-40af-8bd3-1fdacbe00ca3","type":"ToolEvents"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":59},"x_start":{"value":59},"y_end":{"value":0.9},"y_start":{"value":0.5849777036448012}},"id":"96f0e298-d550-4b46-922f-a4ed992d768a","type":"Arrow"},{"attributes":{"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"}},"id":"b8f01fbc-7145-4e2e-8500-fe7dd5d08650","type":"SaveTool"},{"attributes":{"axis_label":"ratings","formatter":{"id":"d25072ea-a7ef-4ca1-9bf4-fe2d0eb72b2a","type":"BasicTickFormatter"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"ticker":{"id":"854c8e62-310d-48b1-94eb-f5e915c89a8c","type":"BasicTicker"}},"id":"8725351e-d6aa-4a8c-a076-279691d7b5b6","type":"LinearAxis"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":38},"x_start":{"value":38},"y_end":{"value":0.8},"y_start":{"value":0.9054791880442197}},"id":"3cccaf54-2846-48dd-9ebc-24a0f1679284","type":"Arrow"},{"attributes":{"end":null,"line_color":{"value":"orange"},"plot":{"id":"0457cfca-659c-4422-876b-5a9400eb9386","subtype":"Figure","type":"Plot"},"source":null,"start":null,"x_end":{"value":32},"x_start":{"value":32},"y_end":{"value":0.0},"y_start":{"value":0.7422573903987334}},"id":"4b515852-2a6b-419b-a9fb-cbc920dfdcf6","type":"Arrow"},{"attributes":{"bottom_units":"screen","fill_alpha":{"value":0.5},"fill_color":{"value":"lightgrey"},"left_units":"screen","level":"overlay","line_alpha":{"value":1.0},"line_color":{"value":"black"},"line_dash":[4,4],"line_width":{"value":2},"plot":null,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"4ae2eb6f-2e14-4345-894f-dc0259a109e1","type":"BoxAnnotation"}],"root_ids":["0457cfca-659c-4422-876b-5a9400eb9386"]},"title":"Bokeh Application","version":"0.12.3"}};
                var render_items = [{"docid":"ecfea1dd-721d-4714-b7c7-a3cda7b2ac8f","elementid":"c3f3106e-f28c-4c18-b27d-cf0f4bbacda8","modelid":"0457cfca-659c-4422-876b-5a9400eb9386"}];
                
                Bokeh.embed.embed_items(docs_json, render_items);
            });
        });
        </script>
    </body>
</html>