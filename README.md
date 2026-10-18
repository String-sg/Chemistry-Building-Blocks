# Chemistry Building Blocks

**Developer:** Kuang Wen<br>
**Product operations and documentation:** Kahhow

A Microsoft Word desktop toolkit that helps chemistry teachers create molecules and diagrams by reusing prepared shapes instead of drawing them from scratch. The contribution is the chemistry-specific diagram collection and its Word workflow, built on Word's existing building-block functionality.

## History and current status

- **5 January 2023:** Kuang Wen [published the toolkit files](https://github.com/String-sg/Chemistry-Building-Blocks/commit/1aaec59f46b70789f3be4a5259717140c2c0669a). This is the first publication recorded in this repository; development may have started earlier.
- **January 2023:** Kahhow added installation documentation and screenshots. The last change before this documentation correction was [27 January 2023](https://github.com/String-sg/Chemistry-Building-Blocks/commit/e90e2334bf07d6e827b0adde76ff99f74b6902cf).
- **January 2024:** A [separate v2 experiment](https://github.com/String-sg/chemistry-building-blocks-v2) explored selecting existing diagrams from a natural-language query. Its relationship to this toolkit is described below.

As of **18 October 2026**, the distributed templates remain the January 2023 toolkit. The documented platform is **desktop Microsoft Word on Windows**. The original documentation does not record tested Word builds, and compatibility with current Word releases has not been revalidated. Mac, Linux and Word for the web are outside the documented installation workflow.

The intended benefit remains less repeated diagram drawing when preparing chemistry materials. No measured time-saving or current classroom-usage results are included in this repository.

## Files to download

Download both templates before installation:

| File | Purpose |
| --- | --- |
| [Chemistry Building Blocks.dotx](Chemistry%20Building%20Blocks.dotx) | Chemistry diagram building-block collection |
| [Chemistry Building Blocks_StartUp_v5.dotm](Chemistry%20Building%20Blocks_StartUp_v5.dotm) | Macro-enabled startup template with the toolkit's ribbon button |
| [Chemistry Building Blocks Instructions.pdf](Chemistry%20Building%20Blocks%20Instructions.pdf) | Original eight-page illustrated installation guide |
| [ReadMe.txt](ReadMe.txt) | Original change note: synthesis boxes added; electrolytic cell listed as a next update |

## Setup and installation on Windows

The steps below preserve the workflow in the original guide and include installation of **both** templates. The historical screenshots and PDF refer to `StartUp_v1.dotm`; use the supplied **`Chemistry Building Blocks_StartUp_v5.dotm`** instead.

### 1. Install the startup template

1. In Word, go to **File > Options**.

   <img width="797" alt="Word File Options" src="https://user-images.githubusercontent.com/44336310/212552067-5172ea05-ff7f-4cb1-b4f3-6164c833b5ad.png">

2. Select **Advanced**, scroll to **General**, then select **File Locations**.

   <img width="793" alt="Advanced options and File Locations" src="https://user-images.githubusercontent.com/44336310/212552117-16e1d1a3-243a-4c7e-bd05-01f4807f3acd.png">

3. Double-click **Startup**.

   <img width="794" alt="Startup file location" src="https://user-images.githubusercontent.com/44336310/212552139-d48196af-20ce-4bea-811a-4795b237930b.png">

4. Copy `Chemistry Building Blocks_StartUp_v5.dotm` from your download folder into the Startup folder opened by Word. The dialog may filter the copied file out of view; the original guide notes this behaviour. Click **OK** to exit the dialogs.

   <img width="797" alt="Copying the startup template; historical screenshot shows v1" src="https://user-images.githubusercontent.com/44336310/212552158-bcb38af3-c91a-413a-b826-a3d0657d42a6.png">

5. Return to **File > Options > Add-ins**.

   <img width="793" alt="Word Add-ins options" src="https://user-images.githubusercontent.com/44336310/212552172-25dbf609-6617-467d-af5c-e2b78f6e1fa5.png">

6. Under **Manage**, select **Templates** and click **Go**.

   <img width="795" alt="Manage Templates" src="https://user-images.githubusercontent.com/44336310/212552185-a9eddbd9-b130-4878-b795-242c5ae092ef.png">

7. Ensure `Chemistry Building Blocks_StartUp_v5.dotm` is checked, then click **OK**.

   <img width="718" alt="Enabled startup template; historical screenshot shows v1" src="https://user-images.githubusercontent.com/44336310/212552202-36604f35-0cb2-4a35-aa34-12933c0bff63.png">

### 2. Install the diagram building blocks

The original PDF covers this second part on **pages 6-8**:

1. Return to **File > Options > Advanced > General > File Locations**.
2. Double-click **Templates**, then click the **Up** arrow to reach its parent Microsoft folder.
3. Open **Document Building Blocks > 1033 > 16**.
4. Copy `Chemistry Building Blocks.dotx` into that folder. As with the Startup dialog, the file may disappear from the filtered view.
5. Click **OK** and exit the dialogs.

`1033 > 16` is the folder layout shown in the original guide. Other Word language/version folder layouts have not been validated here.

The startup template defines a **Chemistry Building Blocks** button in the **Building Blocks** group on Word's **Home** tab.

## Relationship to v2

[chemistry-building-blocks-v2](https://github.com/String-sg/chemistry-building-blocks-v2) is a dependent retrieval prototype, not a self-contained successor. Its [VBA fragment](https://github.com/String-sg/chemistry-building-blocks-v2/blob/main/Code.txt) lists four diagram labels, uses a placeholder external API endpoint, and implements only the exothermic-diagram insertion branch. It also requires an `InsertBuildingBlock` implementation and existing Word building blocks. It does not replace the templates distributed here.

## Maintenance and product consideration

A curated collection of reusable, editable chemistry diagrams may still be useful for worksheet preparation. The next decision is whether maintaining this Windows workflow or making the same assets easier to find and insert best serves current teachers.

- [ ] Record installation and diagram-insertion results on a current Word/Windows version.
- [ ] Compare the existing workflow with a simpler diagram catalogue and record teacher preparation effort.
- [ ] Before moving to a self-contained successor, verify that it includes the required assets and functionality, and preserve author credits, publication dates and links to both repositories.

The templates remain available here while that assessment is open; v2's existence alone is not a reason to retire this base toolkit.
