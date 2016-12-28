---
layout: page
title:  GML geometric primitives examples
permalink: /samplefiles/geomprimitives/
---

# GML geometric primitives examples

* Table of Content
{:toc}


- - - 

## gml:MultiSurface

<i class="fa fa-download" aria-hidden="true"></i> <a href="one_multisurface.gml">one_multisurface.gml</a>

<div class="row">
  <div class="col-md-3 col-sm-6">
    <img class="img-responsive" src="one_multisurface.jpg" alt="...">
  </div>
  <div class="col-md-9 col-sm-6">
    {% highlight xml linenos %}
    <gml:MultiSurface>
      <gml:surfaceMember>
        <gml:Polygon>
          <gml:exterior>
            <gml:LinearRing>
              <gml:pos>0.00 0.00 0.00</gml:pos>
              <gml:pos>0.00 1.00 0.00</gml:pos>
              <gml:pos>1.00 1.00 0.00</gml:pos>
              <gml:pos>1.00 0.00 0.00</gml:pos>
              <gml:pos>0.00 0.00 0.00</gml:pos>
            </gml:LinearRing>
          </gml:exterior>
        </gml:Polygon>
      </gml:surfaceMember>
    </gml:MultiSurface>
    {% endhighlight %}
  </div>
</div>


- - - 

## gml:Solid

<i class="fa fa-download" aria-hidden="true"></i> <a href="one_solid.gml">one_solid.gml</a>

<div class="row">
  <div class="col-md-3 col-sm-6">
    <img class="img-responsive" src="one_solid.jpg" alt="...">
  </div>
  <div class="col-md-9 col-sm-6">
  {% highlight xml linenos %}
<gml:Solid>
  <gml:exterior>
    <gml:CompositeSurface>
      <gml:surfaceMember>
        <gml:Polygon>
          <gml:exterior>
            <gml:LinearRing>
              <gml:pos>0.0 0.0 0.0</gml:pos>
              <gml:pos>0.0 1.0 0.0</gml:pos>
              <gml:pos>1.0 1.0 0.0</gml:pos>
              <gml:pos>1.0 0.0 0.0</gml:pos>
              <gml:pos>0.0 0.0 0.0</gml:pos>
            </gml:LinearRing>
          </gml:exterior>
        </gml:Polygon>
      </gml:surfaceMember>
      ...
    </gml:exterior>
  </gml:CompositeSurface>
</gml:Solid>
{% endhighlight %}
</div>
</div>

- - -

## gml:MultiSolid

<i class="fa fa-download" aria-hidden="true"></i> <a href="one_multisolid.gml">one_multisolid.gml</a>

<div class="row">
  <div class="col-md-3 col-sm-6">
    <img class="img-responsive" src="one_multisolid.jpg" alt="...">
  </div>
  <div class="col-md-9 col-sm-6">
  {% highlight xml linenos %}
<gml:MultiSolid>
  <gml:solidMember>
    <gml:Solid>
      <gml:exterior>
        <gml:CompositeSurface>
          <gml:surfaceMember>
            <gml:Polygon>
              <gml:exterior>
                <gml:LinearRing>
                  <gml:pos>0.00 0.00 0.00</gml:pos>
                  <gml:pos>0.00 100.00 0.00</gml:pos>
                  <gml:pos>100.00 100.00 0.00</gml:pos>
                  <gml:pos>100.00 0.00 0.00</gml:pos>
                  <gml:pos>0.00 0.00 0.00</gml:pos>
                </gml:LinearRing>
              </gml:exterior>
            </gml:Polygon>
          </gml:surfaceMember>
          <gml:surfaceMember>
          ...
          </gml:surfaceMember>
        </gml:CompositeSurface>
      </gml:exterior>
    </gml:Solid>
  </gml:solidMember>
  <gml:solidMember>
    <gml:Solid>
    ...
    </gml:Solid>
  </gml:solidMember>
</gml:MultiSolid>
{% endhighlight %}
</div>
</div>

- - -

## gml:CompositeSolid

<i class="fa fa-download" aria-hidden="true"></i> <a href="one_compositesolid.gml">one_compositesolid.gml</a>

<div class="row">
  <div class="col-md-3 col-sm-6">
    <img class="img-responsive" src="one_compositesolid.jpg" alt="...">
  </div>
  <div class="col-md-9 col-sm-6">
  {% highlight xml linenos %}
<gml:CompositeSolid>
  <gml:solidMember>
    <gml:Solid>
      <gml:exterior>
        <gml:CompositeSurface>
          <gml:surfaceMember>
            <gml:Polygon>
              <gml:exterior>
                <gml:LinearRing>
                  <gml:pos>0.00 0.00 0.00</gml:pos>
                  <gml:pos>0.00 100.00 0.00</gml:pos>
                  <gml:pos>100.00 100.00 0.00</gml:pos>
                  <gml:pos>100.00 0.00 0.00</gml:pos>
                  <gml:pos>0.00 0.00 0.00</gml:pos>
                </gml:LinearRing>
              </gml:exterior>
            </gml:Polygon>
          </gml:surfaceMember>
          <gml:surfaceMember>
          ...
          </gml:surfaceMember>
        </gml:CompositeSurface>
      </gml:exterior>
    </gml:Solid>
  </gml:solidMember>
  <gml:solidMember>
    <gml:Solid>
    ...
    </gml:Solid>
  </gml:solidMember>
</gml:CompositeSolid>
{% endhighlight %}
</div>
</div>
