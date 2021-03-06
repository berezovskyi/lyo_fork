# Lyo Validation library

The library validates RDF resources against constraints defined either as [SHACL](https://www.w3.org/TR/shacl/) or [OSLC Resource Shapes](http://docs.oasis-open.org/oslc-core/oslc-core/v3.0/cs01/part6-resource-shape/oslc-core-v3.0-cs01-part6-resource-shape.html).

## Getting started

Add a dependency for the library:

```xml
<dependency>
    <groupId>org.eclipse.lyo</groupId>
    <artifactId>lyo-validation</artifactId>
    <version>${version.lyo}</version>
</dependency>
```

Start by reading the library's main interface class [`Validator`](https://download.eclipse.org/lyo/docs/all/latest/apidocs/org/eclipse/lyo/validation/Validator.html) on Javadoc.

You can also review the library's [unit test cases](src/test/java/org/eclipse/lyo/validation) that shows how to use this interface. 

Finally, you can review the [sample application](src/test/java/org/eclipse/lyo/validation/ValidationExample.java), which shows 3 validation examples, where:

* an RDF resource (jena model) is validated against a SHACL shape (another jena model).
* An java object (representing an RDF resource) is validated against SHACL annotations defined on its Java class.
* An java object (representing an RDF resource) is validated against OSLC annotations defined on its Java class.

