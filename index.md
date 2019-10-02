---
layout: default
---

# Curso de Neuroimágenes de SLAN 2019
**Pablo A. Reyes** reyes.p @ javeriana.edu.co (sin espacios)


La siguiente página ofrece las herramientas y ejemplos básicos para poder realizar una introducción a la visualización, análisis y procesamiento básico de imágenes cerebrales obtenidas por MRI. Cabe anotar que esta es una selección puntual de alguos programas que me han servido en mi experiencia. Existen una basta cantidad de opciones que dependen en gran parte del nivel y experiencia del usuario.


# Bases de Datos y OpenScience

Existen diversas bases de datos de imágenes de MRI que son accesibles de manera libre.

**Bases de imagenes**
1. <a href="https://openneuro.org">Open Neuro</a> : Base de datos multimodales (MRI, EEG, MEG), permite tanto bajar como subir estudio. Actualmente cuenta con 287 bases de datos.
2. <a href="https://ida.loni.usc.edu/login.jsp">Image & Data Archive IDA</a>: ABIDE (Autismo), ABVIB (Envejecimiento), ADNI (Alzheimer), ADNIDOD (Veteranos), AIBL, BIOFIND, ICBM (consorcio de mapeo cerebral), GSP (Genómica), HCP (Human connectome project), PPMI (Parkinson), NIFD (Demencia Frontotemporal).
3. <a href="https://www.humanconnectome.org">Conectoma Humano</a>: Iniciativa que comenzó con un estudio masivo de mapeo cerebral en sujetos sanos y se ha extendido a 3 escenarios importantes:
- HCP adultos jóvenes = 1200
- HCP curso vital
  - Bebes
  - Infancia
  - Adultos
  - Prenatal y neonatal
- Estudios clínicos
  - Amish
  - Epilepsia
  - Ansiedad
  - Alzheimer
  - Ceguera y baja visión
4. <a href="http://www.oasis-brains.org">OASIS</a>: Base de datos de MRI sobre sujetos normales y pacientes con enfermedad de Alzheimer. Principalmente imágenes de tipo estructural.


**Meta análisis y revisiones**
1. <a href="https://neurovault.org">NeuroVault</a> : Base de datos de MRI de resultados de análisis (mapas de conectividad).
2. <a href="https://neurosynth.org">Neurosynth</a> : Plataforma para realización de metanálisis de estudios de fMRI, la base d ela información proviene principalmente de las coordenadas de activación reportadas por los artículos publicados.


# Visualizadores
_Dicom_

La imágenes salen del scanner en formato DICOM, este formato si bien es útil para transmitir imágenes convservando detalles del paciente y de la máquina; tienen serios problemas para ser manipulados en ambientes de investigación. En general para análisis de neuroimágenes se prefiere covertir estos archivos dicom a NIFTI.

1. <a href="https://www.osirix-viewer.com">Osirix</a> : Visor médico con amplias funcionalidades de imágenes DICOM, solo funciona sobre MAC.
2. <a href="https://nroduit.github.io/en/">Weasis</a> : Visor médico de acceso libre.

_NifTI_
Existen multiples programas que permiten visualizar imágenes NIFTI, algunos de ellos estan para MATLAB, Python o pueden funcionar de manera independiente.

1. <a href="http://www.itksnap.org/pmwiki/pmwiki.php">ITK-Snap</a> : Visualiza imágenes en diferentes formatos, tanto NIFTI como otras un poco mas antiguas como HDR/IMG, y formatos VTK. Una de sus principales ventajas es la posibilidad de sobreponer máscaras, asi como también realizar segmentaciones de regiones de manera manual o semiautomática.
2. <a href="https://www.mccauslandcenter.sc.edu/mricrogl/">MRIcroGL</a> : Similar al anterior pero enfocado en renderización (3D), también permite sobreponer máscaras y realizar segmentaciones de manera manual.
3. <a href="http://ric.uthscsa.edu/mango/papaya.html">Papaya</a> : Se trata de un visor basado en JavaScript que permite convertir a otros formatos e incluye algunas formas de preanálisis básicas como segmentación de cráneo.

## Tutorial: Convertir una imagen DICOM a NIFTI


{% include youtubePlayer.html id=F_cskbDONr0 %}




> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

```sh
cp dirrectoy testy
rm mr

```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
