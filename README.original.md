

# About

* Potree is a free open-source WebGL based point cloud renderer for large point clouds. It is based on the [TU Wien Scanopy project](https://www.cg.tuwien.ac.at/research/projects/Scanopy/) and research projects [Harvest4D](https://harvest4d.org/), [GCD Doctoral College](https://gcd.tuwien.ac.at/) and [Superhumans](https://www.cg.tuwien.ac.at/research/projects/Superhumans/).
* Newest information and work in progress is usually available on [twitter](https://twitter.com/m_schuetz)
* Contact: Markus Schütz (mschuetz@potree.org)
* References: 
    * [Potree: Rendering Large Point Clouds in Web Browsers](https://www.cg.tuwien.ac.at/research/publications/2016/SCHUETZ-2016-POT/SCHUETZ-2016-POT-thesis.pdf) (2016)
    * [Fast Out-of-Core Octree Generation for Massive Point Clouds](https://www.cg.tuwien.ac.at/research/publications/2020/SCHUETZ-2020-MPC/) (2020)
    
<a href="http://potree.org/wp/demo/" target="_blank"> ![](./docs/images/potree_screens.png) </a>

# Getting Started

### Install on your PC

Install [node.js](http://nodejs.org/)

Install dependencies, as specified in package.json, and create a build in ./build/potree.

```bash
npm install
```

### Run on your PC

Use the `npm start` command to 

* create ./build/potree 
* watch for changes to the source code and automatically create a new build on change
* start a web server at localhost:1234. 

Go to http://localhost:1234/examples/ to test the examples.

### Deploy to a server

* Simply upload the Potree folderm with all your point clouds, the build directory, and your html files to a web server.
* It is not required to install node.js on your webserver. All you need is to host your files online. 

### Convert Point Clouds to Potree Format

Download [PotreeConverter](https://github.com/potree/PotreeConverter) and run it like this:

    ./PotreeConverter.exe C:/pointclouds/data.las -o C:/pointclouds/data_converted

Copy the converted directory into &lt;potreeDirectory&gt;/pointclouds/data_converted. Then, duplicate and rename one of the examples and modify the path in the html file to your own point cloud.

# Downloads

* [Potree](https://github.com/potree/potree/releases)
* [PotreeConverter ](https://github.com/potree/PotreeConverter/releases) - Convert your point cloud to the Potree format.
* [PotreeDesktop ](https://github.com/potree/PotreeDesktop/releases) - Desktop version of Potree. Allows drag&drop of point clouds into the viewer.

# Examples

<table>
	<tr>
		<td style="padding: 0px">
			<a href="http://potree.org/potree/examples/viewer.html" target="_blank">
				<img src="examples/thumbnails/viewer.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/ca13.html" target="_blank">
				<img src="examples/thumbnails/ca13.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/cesium_retz.html" target="_blank">
				<img src="examples/thumbnails/cesium_retz.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/classifications.html" target="_blank">
				<img src="examples/thumbnails/classifications.jpg" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/features_sorvilier.html" target="_blank">
				<img src="examples/thumbnails/features_sorvilier.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/toolbar.html" target="_blank">
				<img src="examples/thumbnails/toolbar.jpg" width="100%" />
			</a>
		</td>
	</tr>
	<tr>
		<th>Basic Viewer</th><th>CA13 (18 billion Points)</th><th>Retz (Potree + Cesium)</th><th>Classifications</th><th>Various Features</th><th>Toolbar</th>
	</tr>
</table>

<details>
<summary>More Examples</summary>


<table>
	<tr>
		<td>
			<a href="http://potree.org/potree/examples/load_project.html" target="_blank">
				<img src="examples/thumbnails/load_project.jpg" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/matcap.html" target="_blank">
				<img src="examples/thumbnails/matcap.jpg" width="100%" />
			</a>
		</td><td>
			<a href="https://potree.org/potree/examples/vr_heidentor.html" target="_blank">
				<img src="examples/thumbnails/heidentor.jpg" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/heidentor.html" target="_blank">
				<img src="examples/thumbnails/heidentor.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/lion.html" target="_blank">
				<img src="examples/thumbnails/lion.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/lion_las.html" target="_blank">
				<img src="examples/thumbnails/lion_las.png" width="100%" />
			</a>
		</td>
	</tr>
	<tr>
		<th>Load Project</th><th>Matcap</th><th>Virtual Reality</th><th>Heidentor</th><th>Lion</th><th>Lion LAS</th>
	</tr><tr>
		<td>
			<a href="http://potree.org/potree/examples/lion_laz.html" target="_blank">
				<img src="examples/thumbnails/lion_las.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/ept.html" target="_blank">
				<img src="examples/thumbnails/lion.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/ept_binary.html" target="_blank">
				<img src="examples/thumbnails/lion_las.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/ept_zstandard.html" target="_blank">
				<img src="examples/thumbnails/lion_las.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/clipping_volume.html" target="_blank">
				<img src="examples/thumbnails/clipping_volume.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/oriented_images.html" target="_blank">
				<img src="examples/thumbnails/oriented_images.jpg" width="100%" />
			</a>
		</td>
	</tr>
	<tr>
		<th>Lion LAZ</th><th>EPT</th><th>EPT Binary</th><th>EPT zstandard</th><th>Clipping Volume</th><th>Oriented Images</th>
	</tr><tr>
		<td>
			<a href="http://potree.org/potree/examples/elevation_profile.html" target="_blank">
				<img src="examples/thumbnails/elevation_profile.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/measurements.html" target="_blank">
				<img src="examples/thumbnails/measurements.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/meshes.html" target="_blank">
				<img src="examples/thumbnails/meshes.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/multiple_pointclouds.html" target="_blank">
				<img src="examples/thumbnails/multiple_point_clouds.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/camera_animation.html" target="_blank">
				<img src="examples/thumbnails/camera_animation.jpg" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/features_ca13.html" target="_blank">
				<img src="examples/thumbnails/features_ca13.png" width="100%" />
			</a>
		</td>
	</tr>
	<tr>
		<th>Elevation Profile</th><th>Measurements</th><th>Meshes</th><th>Multiple Point Clouds</th><th>Camera Animation</th><th>Features (CA13)</th>
	</tr><tr>
		<td>
			<a href="http://potree.org/potree/examples/annotations.html" target="_blank">
				<img src="examples/thumbnails/annotations.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/annotation_hierarchy.html" target="_blank">
				<img src="examples/thumbnails/annotation_hierarchy.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/animation_paths.html" target="_blank">
				<img src="examples/thumbnails/animation_paths.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/shapefiles.html" target="_blank">
				<img src="examples/thumbnails/shapefiles.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/cesium_ca13.html" target="_blank">
				<img src="examples/thumbnails/cesium_ca13.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/geopackage.html" target="_blank">
				<img src="examples/thumbnails/geopackage.jpg" width="100%" />
			</a>
		</td>
	</tr>
	<tr>
		<th>Annotations</th><th>Hierarchical Annotations</th><th>Animation Path</th><th>Shapefiles</th><th>Cesium CA13</th><th>Geopackage</th>
	</tr><tr>
		<td>
			<a href="http://potree.org/potree/examples/cesium_sorvilier.html" target="_blank">
				<img src="examples/thumbnails/cesium_sorvilier.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/custom_sidebar_section.html" target="_blank">
				<img src="examples/thumbnails/custom_sidebar_section.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/embedded_iframe.html" target="_blank">
				<img src="examples/thumbnails/embedded_iframe.png" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/gradient_colors.html" target="_blank">
				<img src="examples/thumbnails/gradient_colors.png" width="100%" />
			</a>
		</td>
	</tr>
	<tr>
		<th>Cesium Sorvilier</th><th>Custom Sidebar Section</th><th>Embedded Iframe</th><th>Gradient Colors</th>
	</tr>
</table>

# VR

<table>
	<tr>
		<td>
			<a href="https://potree.org/potree/examples/vr_heidentor.html" target="_blank">
				<img src="examples/thumbnails/heidentor.jpg" width="100%" />
			</a>
		</td><td>
			<a href="https://potree.org/potree/examples/vr_eclepens.html" target="_blank">
				<img src="examples/thumbnails/eclepens.jpg" width="100%" />
			</a>
		</td><td>
			<a href="https://potree.org/potree/examples/vr_morro_bay.html" target="_blank">
				<img src="examples/thumbnails/ca13.png" width="100%" />
			</a>
		</td><td>
			<a href="https://potree.org/potree/examples/vr_lion.html" target="_blank">
				<img src="examples/thumbnails/lion.png" width="100%" />
			</a>
		</td><td>
			<a href="https://potree.org/potree/examples/vr_dechen_cave.html" target="_blank">
				<img src="examples/thumbnails/dechen_cave.jpg" width="100%" />
			</a>
		</td>
	</tr>
	<tr>
		<th>Heidentor</th><th>Eclepens</th><th>Morro Bay</th><th>Lion</th><th>Dechen Cave</th>
	</tr>
</table>

# Showcase

<table>
	<tr>
		<td>
			<a href="http://potree.org/potree/examples/showcase/matterhorn.html" target="_blank">
				<img src="examples/thumbnails/matterhorn.jpg" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/showcase/retz.html" target="_blank">
				<img src="examples/thumbnails/retz.jpg" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/showcase/lake_tahoe.html" target="_blank">
				<img src="examples/thumbnails/lake_tahoe.jpg" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/showcase/sorvilier.html" target="_blank">
				<img src="examples/thumbnails/vol_total.jpg" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/showcase/grab_15.html" target="_blank">
				<img src="examples/thumbnails/grab_15.jpg" width="100%" />
			</a>
		</td><td>
			<a href="http://potree.org/potree/examples/showcase/tern_auscover_chowilla.html" target="_blank">
				<img src="examples/thumbnails/chowilla.jpg" width="100%" />
			</a>
		</td>
	</tr>
	<tr>
		<th>Matterhorn</th><th>Retz</th><th>Lake Tahoe</th><th>Sorvilier</th><th>Grave</th><th>Chowilla</th>
	</tr>
</table>

<details>
... (truncated)
