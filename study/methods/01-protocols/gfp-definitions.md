# GFP definitions

## eGFP

[Enhanced GFP][2y0g] (eGFP), first introduced by [Heim et al.][egfp paper], has `S65T` and `F64L` mutations from the wild type protein.

!!! quote "2Y0G"
    <div id="2Y0G-view" class="mol-container"></div>

<script>
document.addEventListener('DOMContentLoaded', (event) => {
    const viewer = molstar.Viewer.create('2Y0G-view', {
        layoutIsExpanded: false,
        layoutShowControls: false,
        layoutShowRemoteState: false,
        layoutShowSequence: true,
        layoutShowLog: false,
        layoutShowLeftPanel: false,
        viewportShowExpand: true,
        viewportShowSelectionMode: true,
        viewportShowAnimation: false,
        pdbProvider: 'rcsb',
    }).then(viewer => {
        // viewer.loadPdb("2Y0G");
        viewer.loadSnapshotFromUrl("/misc/002-molstar-states/2Y0G.molj", "molj");
    });
});
</script>

## roGFP

The [redox-sensitive GFP][rogfp paper] (roGFP) is derived from [eGFP](#egfp) with two additional mutations: `S147C` and `Q204C`.
Introduced as roGFP2 [Hanson et al.][rogfp paper], this forms a reversible formation of a [reduced][1jc0] and [oxidized][1jc1] disulfide bridge between `147` and `204`.

!!! note

    Due to renumbering residues in our [protein preparation pipeline](../02-protein-prep.md), these residues are `145` and `202` in our simulations.

### Reduced form

[1JC0][1jc0] shows the reduced (i.e., broken) form of `147`-`204` disulfide bond.

!!! quote "1JC0"
    <div id="1JC0-view" class="mol-container"></div>

<script>
document.addEventListener('DOMContentLoaded', (event) => {
    const viewer = molstar.Viewer.create('1JC0-view', {
        layoutIsExpanded: false,
        layoutShowControls: false,
        layoutShowRemoteState: false,
        layoutShowSequence: true,
        layoutShowLog: false,
        layoutShowLeftPanel: false,
        viewportShowExpand: true,
        viewportShowSelectionMode: true,
        viewportShowAnimation: false,
        pdbProvider: 'rcsb',
    }).then(viewer => {
        // viewer.loadPdb("1JC0");
        viewer.loadSnapshotFromUrl("/misc/002-molstar-states/1JC0.molj", "molj");
    });
});
</script>

### Oxidized form

[1JC1][1jc1] shows the oxidized (i.e., formed) form of `147`-`204` disulfide bond.

!!! quote "1JC1"
    <div id="1JC1-view" class="mol-container"></div>

<script>
document.addEventListener('DOMContentLoaded', (event) => {
    const viewer = molstar.Viewer.create('1JC1-view', {
        layoutIsExpanded: false,
        layoutShowControls: false,
        layoutShowRemoteState: false,
        layoutShowSequence: true,
        layoutShowLog: false,
        layoutShowLeftPanel: false,
        viewportShowExpand: true,
        viewportShowSelectionMode: true,
        viewportShowAnimation: false,
        pdbProvider: 'rcsb',
    }).then(viewer => {
        // viewer.loadPdb("1JC1");
        viewer.loadSnapshotFromUrl("/misc/002-molstar-states/1JC1.molj", "molj");
    });
});
</script>

[egfp paper]: https://doi.org/10.1038/373663b0
<h1 align="center">MetalFlare</h1>

<h4 align="center">Computational investigation of a Cu(I)-sensing green fluorescent protein</h4>

<p align="center">
    <a href="https://github.com/durrantlab/metalflare/releases">
        <img src="https://img.shields.io/github/v/release/durrantlab/metalflare" alt="GitHub release (latest by date)">
    </a>
    <a href="https://github.com/durrantlab/metalflare/" target="_blank">
        <img src="https://img.shields.io/github/repo-size/durrantlab/metalflare" alt="GitHub repo size">
    </a>
</p>

TODO:

[1jc0]: https://www.rcsb.org/structure/1jc0
[1jc1]: https://www.rcsb.org/structure/1jc1
[rogfp paper]: https://doi.org/10.1074/jbc.M312846200
[2y0g]: https://www.rcsb.org/structure/2y0g
