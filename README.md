# Angular Grid with DOM Virtualization and Paging

This Angular application demonstrates a Syncfusion Grid configured with DOM
virtualization and paging. The grid requests up to 100,000 employee records from
the Syncfusion remote data service and renders rows as needed while you scroll.
Paging is enabled with a default page size of 100 and options for 500 and 1,000
rows per page.

The grid also demonstrates sorting and checkbox filtering, along with custom
employee-name and status templates. DOM virtualization uses a row buffer of 10.

## Requirements

- Node.js and npm

## Run the application

Install dependencies and start the Angular development server:

```bash
npm install
npm start
```

Open [http://localhost:4200](http://localhost:4200) in your browser. The grid
uses the Syncfusion production data service at
`https://services.syncfusion.com/angular/production/`.

## Build

```bash
npm run build
```

The production build is written to `dist/angular18/`.

## Grid configuration

The example's grid is defined in `src/app/app.component.html`. The component in
`src/app/app.component.ts` configures the remote data source, requests a data
count of 100,000, sets the page-size choices, and sets the DOM virtualization
row buffer. Paging is enabled with `allowPaging`, and DOM virtualization with
`enableDomVirtualization`.
