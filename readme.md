### Converts a nodeset to string, especially useful for json conversions.

===================================================================================

Copyright 2011, Thomas Appel, http://thomas-appel.com, mail(at)thomas-appel.com
dual licensed under MIT and GPL license
http://dev.thomas-appel.com/licenses/mit.txt
http://dev.thomas-appel.com/licenses/gpl.txt

===================================================================================

### Example usage:

(convert a exsl nodeset to string: )
___

	<xsl:variable name="somelink">
		<a href="{url}" class="some-class"><xsl:value-of select="name"/></a>
	</xsl:variable>
	<xsl:apply-templates select="exsl:node-set($somelink)/* | exsl:node-set($some-link)/text()" mode="nodetostring"/>
___

(convert xml noset to string: )
___

	<xsl:apply-templates select="node | node[text()" mode="nodetostring"/>

