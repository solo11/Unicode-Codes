---
datapackage:
  title: Unicode Codes
  description: The Unicode Consortium is the standards body for the internationalization of software and services. Deployed on more than 20 billion devices around the world, Unicode also provides the solution for internationalization and the architecture to support localization.
  created: 2024-01-01
  updated: 2024-01-31
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  sources:
  - path: https://home.unicode.org/
    title: Link to data source
  resources:
  - name: unicode-codes
    title: Unicode codes
    description: Unicode codes
    lastModified: 2024-10-10
    path: data.csv
---


<p>The following table describes the format and meaning of each field in a data entry in 
the UnicodeData. Fields which contain normative information are so indicated.</p>

<table BORDER="0" CELLSPACING="2" CELLPADDING="0">
  <tr>
    <th VALIGN="TOP" ALIGN="LEFT"><p ALIGN="LEFT">Field</th>
    <th VALIGN="TOP" ALIGN="LEFT"><p ALIGN="LEFT">Name</th>
    <th VALIGN="TOP" ALIGN="LEFT"><p ALIGN="LEFT">Status</th>
    <th VALIGN="TOP" ALIGN="LEFT"><p ALIGN="LEFT">Explanation</th>
  </tr>
  <tr>
    <th VALIGN="TOP">0</th>
    <td VALIGN="TOP">Code value</td>
    <td VALIGN="TOP">normative</td>
    <td VALIGN="TOP">Code value in 4-digit hexadecimal format.</td>
  </tr>
  <tr>
    <th VALIGN="TOP" BGCOLOR="#c0c0c0">1</th>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">Character name</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">normative</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">These names match exactly the names published in 
    Chapter 7 of the Unicode Standard, Version 2.0, except for the two additional characters.</td>
  </tr>
  <tr>
    <th VALIGN="TOP">2</th>
    <td VALIGN="TOP"><a HREF="ReadMe-3.0.0d3.html#General Category">General category</a></td>
    <td VALIGN="TOP">normative / informative<br>
    (see below)</td>
    <td VALIGN="TOP">This is a useful breakdown into various &quot;character types&quot; which 
    can be used as a default categorization in implementations. See below for a brief 
    explanation.</td>
  </tr>
  <tr>
    <th VALIGN="TOP" BGCOLOR="#c0c0c0">3</th>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0"><a
    HREF="ReadMe-3.0.0d3.html#Canonical Combining Classes">Canonical combining classes</a></td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">normative</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">The classes used for the Canonical Ordering Algorithm 
    in the Unicode Standard. These classes are also printed in Chapter 4 of the Unicode 
    Standard.</td>
  </tr>
  <tr>
    <th VALIGN="TOP">4</th>
    <td VALIGN="TOP"><a HREF="ReadMe-3.0.0d3.html#Bidirectional Category">Bidirectional 
    category</a></td>
    <td VALIGN="TOP">normative</td>
    <td VALIGN="TOP">See the list below for an explanation of the abbreviations used in this 
    field. These are the categories required by the Bidirectional Behavior Algorithm in the 
    Unicode Standard. These categories are summarized in Chapter 3 of the Unicode Standard.</td>
  </tr>
  <tr>
    <th VALIGN="TOP" BGCOLOR="#c0c0c0">5</th>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0"><a HREF="ReadMe-3.0.0d3.html#Character Decomposition">Character 
    decomposition mapping</a></td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">normative</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">In the Unicode Standard, not all of the mappings are 
    full (maximal) decompositions. Recursive application of look-up for decompositions will, 
    in all cases, lead to a maximal decomposition. The decomposition mappings match exactly 
    the decomposition mappings published with the character names in the Unicode Standard.</td>
  </tr>
  <tr>
    <th VALIGN="TOP">6</th>
    <td VALIGN="TOP">Decimal digit value</td>
    <td VALIGN="TOP">normative</td>
    <td VALIGN="TOP">This is a numeric field. If the character has the decimal digit property, 
    as specified in Chapter 4 of the Unicode Standard, the value of that digit is represented 
    with an integer value in this field</td>
  </tr>
  <tr>
    <th VALIGN="TOP" BGCOLOR="#c0c0c0">7</th>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">Digit value</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">normative</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">This is a numeric field. If the character represents a 
    digit, not necessarily a decimal digit, the value is here. This covers digits which do not 
    form decimal radix forms, such as the compatibility superscript digits</td>
  </tr>
  <tr>
    <th VALIGN="TOP">8</th>
    <td VALIGN="TOP">Numeric value</td>
    <td VALIGN="TOP">normative</td>
    <td VALIGN="TOP">This is a numeric field. If the character has the numeric property, as 
    specified in Chapter 4 of the Unicode Standard, the value of that character is represented 
    with an integer or rational number in this field. This includes fractions as, e.g., 
    &quot;1/5&quot; for U+2155 VULGAR FRACTION ONE FIFTH Also included are numerical values 
    for compatibility characters such as circled numbers.</td>
  </tr>
  <tr>
    <th VALIGN="TOP" BGCOLOR="#c0c0c0">8</th>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">Mirrored</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">normative</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">If the character has been identified as a 
    &quot;mirrored&quot; character in bidirectional text, this field has the value 
    &quot;Y&quot;; otherwise &quot;N&quot;. The list of mirrored characters is also printed in 
    Chapter 4 of the Unicode Standard.</td>
  </tr>
  <tr>
    <th VALIGN="TOP">10</th>
    <td VALIGN="TOP">Unicode 1.0 Name</td>
    <td VALIGN="TOP">informative</td>
    <td VALIGN="TOP">This is the old name as published in Unicode 1.0. This name is only 
    provided when it is significantly different from the Unicode 3.0 name for the character.</td>
  </tr>
  <tr>
    <th VALIGN="TOP" BGCOLOR="#c0c0c0">11</th>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">10646 comment field</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">informative</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">This is the ISO 10646 comment field. It is in 
    parantheses in the 10646 names list.</td>
  </tr>
  <tr>
    <th VALIGN="TOP">12</th>
    <td VALIGN="TOP"><a HREF="ReadMe-3.0.0d3.html#Case Mappings">Uppercase mapping</a></td>
    <td VALIGN="TOP">informative</td>
    <td VALIGN="TOP">Upper case equivalent mapping. If a character is part of an alphabet with 
    case distinctions, and has an upper case equivalent, then the upper case equivalent is in 
    this field. See the explanation below on case distinctions. These mappings are always 
    one-to-one, not one-to-many or many-to-one. This field is informative.</td>
  </tr>
  <tr>
    <th VALIGN="TOP" BGCOLOR="#c0c0c0">13</th>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0"><a HREF="ReadMe-3.0.0d3.html#Case Mappings">Lowercase 
    mapping</a></td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">informative</td>
    <td VALIGN="TOP" BGCOLOR="#c0c0c0">Similar to <a HREF="ReadMe-3.0.0d3.html#Case Mappings">Uppercase 
    mapping</a></td>
  </tr>
  <tr>
    <th VALIGN="TOP">14</th>
    <td VALIGN="TOP"><a HREF="ReadMe-3.0.0d3.html#Case Mappings">Titlecase mapping</a></td>
    <td VALIGN="TOP">informative</td>
    <td VALIGN="TOP">Similar to <a HREF="ReadMe-3.0.0d3.html#Case Mappings">Uppercase mapping</a></td>
  </tr>
</table>

<h3><a NAME="General Category"></a>General Category</h3>

<p>The values in this field are abbreviations for the following. Some of the values are 
normative, and some are informative. For more information, see the Unicode Standard.</p>

<p><b>Note:</b> the standard does not assign information to control characters (except for 
certain cases in the Bidirectional Algorithm). Implementations will generally also assign 
categories to certain control characters, notably CR and LF, according to platform 
conventions.</p>

<h4>Normative Categories</h4>

<table BORDER="0" CELLSPACING="2" CELLPADDING="0">
  <tr>
    <th><p ALIGN="LEFT">Abbr.</th>
    <th><p ALIGN="LEFT">Description</th>
  </tr>
  <tr>
    <td ALIGN="CENTER">Lu</td>
    <td>Letter, Uppercase</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Ll</td>
    <td>Letter, Lowercase</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Lt</td>
    <td>Letter, Titlecase</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Mn</td>
    <td>Mark, Non-Spacing</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Mc</td>
    <td>Mark, Spacing Combining</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Me</td>
    <td>Mark, Enclosing</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Nd</td>
    <td>Number, Decimal Digit</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Nl</td>
    <td>Number, Letter</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">No</td>
    <td>Number, Other</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Zs</td>
    <td>Separator, Space</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Zl</td>
    <td>Separator, Line</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Zp</td>
    <td>Separator, Paragraph</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Cc</td>
    <td>Other, Control</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Cf</td>
    <td>Other, Format</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Cs</td>
    <td>Other, Surrogate</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Co</td>
    <td>Other, Private Use</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Cn</td>
    <td>Other, Not Assigned (no characters in the file have this property)</td>
  </tr>
</table>

<h4>Informative Categories</h4>

<table BORDER="0" CELLSPACING="2" CELLPADDING="0">
  <tr>
    <th><p ALIGN="LEFT">Abbr.</th>
    <th><p ALIGN="LEFT">Description</th>
  </tr>
  <tr>
    <td ALIGN="CENTER">Lm</td>
    <td>Letter, Modifier</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Lo</td>
    <td>Letter, Other</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Pc</td>
    <td>Punctuation, Connector</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Pd</td>
    <td>Punctuation, Dash</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Ps</td>
    <td>Punctuation, Open</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Pe</td>
    <td>Punctuation, Close</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Pi</td>
    <td>Punctuation, Initial quote (may behave like Ps or Pe depending on usage)</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Pf</td>
    <td>Punctuation, Final quote (may behave like Ps or Pe depending on usage)</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Po</td>
    <td>Punctuation, Other</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Sm</td>
    <td>Symbol, Math</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Sc</td>
    <td>Symbol, Currency</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">Sk</td>
    <td>Symbol, Modifier</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">So</td>
    <td>Symbol, Other</td>
  </tr>
</table>

<h3><a NAME="Bidirectional Category"></a>Bidirectional Category</h3>

<p>Please refer to Chapter 3 for an explanation of the algorithm for Bidirectional 
Behavior and an explanation of the significance of these categories. An up-to-date version 
can be found on <a HREF="http://www.unicode.org/unicode/reports/tr9/">Unicode Technical 
Report #9</a>. These values are normative.</p>

<h3><a NAME="Character Decomposition"></a>Character Decomposition</h3>

<p>The decomposition is a normative property of a character. The tags supplied with 
certain decomposition mappings generally indicate formatting information. Where no such 
tag is given, the mapping is designated as canonical. Conversely, the presence of a 
formatting tag also indicates that the mapping is a compatibility mapping and not a 
canonical mapping. In the absence of other formatting information in a compatibility 
mapping, the tag is used to distinguish it from canonical mappings.</p>

<p>In some instances a canonical mapping or a compatibility mapping may consist of a 
single character. For a canonical mapping, this indicates that the character is a 
canonical equivalent of another single character. For a compatibility mapping, this 
indicates that the character is a compatibility equivalent of another single character. 
The compatibility formatting tags used are:</p>

<table BORDER="0" CELLSPACING="2" CELLPADDING="0">
  <tr>
    <th>Tag</th>
    <th><p ALIGN="LEFT">Description</th>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;font&gt;&nbsp;&nbsp;</td>
    <td>A font variant (e.g. a blackletter form).</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;noBreak&gt;&nbsp;&nbsp;</td>
    <td>A no-break version of a space or hyphen.</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;initial&gt;&nbsp;&nbsp;</td>
    <td>An initial presentation form (Arabic).</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;medial&gt;&nbsp;&nbsp;</td>
    <td>A medial presentation form (Arabic).</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;final&gt;&nbsp;&nbsp;</td>
    <td>A final presentation form (Arabic).</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;isolated&gt;&nbsp;&nbsp;</td>
    <td>An isolated presentation form (Arabic).</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;circle&gt;&nbsp;&nbsp;</td>
    <td>An encircled form.</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;super&gt;&nbsp;&nbsp;</td>
    <td>A superscript form.</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;sub&gt;&nbsp;&nbsp;</td>
    <td>A subscript form.</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;vertical&gt;&nbsp;&nbsp;</td>
    <td>A vertical layout presentation form.</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;wide&gt;&nbsp;&nbsp;</td>
    <td>A wide (or zenkaku) compatibility character.</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;narrow&gt;&nbsp;&nbsp;</td>
    <td>A narrow (or hankaku) compatibility character.</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;small&gt;&nbsp;&nbsp;</td>
    <td>A small variant form (CNS compatibility).</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;square&gt;&nbsp;&nbsp;</td>
    <td>A CJK squared font variant.</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;fraction&gt;&nbsp;&nbsp;</td>
    <td>A vulgar fraction form.</td>
  </tr>
  <tr>
    <td ALIGN="CENTER">&lt;compat&gt;&nbsp;&nbsp;</td>
    <td>Otherwise unspecified compatibility character.</td>
  </tr>
</table>

<p><b>Reminder: </b>There is a difference between decomposition and decomposition mapping. 
The decomposition mappings are defined in the UnicodeData, while the decomposition (also 
termed &quot;full decomposition&quot;) is defined in Chapter 3 to use those mappings 
recursively. </p>

<ul>
  <li>The canonical decomposition is formed by recursively applying the canonical mappings, 
    then applying the canonical reordering algorithm. </li>
  <li>The compatibility decomposition is formed by recursively applying the canonical <em>and</em> 
    compatibility mappings, then applying the canonical reordering algorithm. </li>
</ul>

<h3><a NAME="Canonical Combining Classes"></a>Canonical Combining Classes</h3>

<table BORDER="0" CELLSPACING="2" CELLPADDING="0">
  <tr>
    <th><p ALIGN="LEFT">Value</th>
    <th><p ALIGN="LEFT">Description</th>
  </tr>
  <tr>
    <td ALIGN="RIGHT">0:</td>
    <td>Spacing, split, enclosing, reordrant, and Tibetan subjoined</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">1:</td>
    <td>Overlays and interior</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">7:</td>
    <td>Nuktas</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">8:</td>
    <td>Hiragana/Katakana voicing marks</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">9:</td>
    <td>Viramas</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">10:</td>
    <td>Start of fixed position classes</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">199:</td>
    <td>End of fixed position classes</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">200:</td>
    <td>Below left attached</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">202:</td>
    <td>Below attached</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">204:</td>
    <td>Below right attached</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">208:</td>
    <td>Left attached (reordrant around single base character)</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">210:</td>
    <td>Right attached</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">212:</td>
    <td>Above left attached</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">214:</td>
    <td>Above attached</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">216:</td>
    <td>Above right attached</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">218:</td>
    <td>Below left</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">220:</td>
    <td>Below</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">222:</td>
    <td>Below right</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">224:</td>
    <td>Left (reordrant around single base character)</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">226:</td>
    <td>Right</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">228:</td>
    <td>Above left</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">230:</td>
    <td>Above</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">232:</td>
    <td>Above right</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">233:</td>
    <td>Double below</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">234:</td>
    <td>Double above</td>
  </tr>
  <tr>
    <td ALIGN="RIGHT">240:</td>
    <td>Below (iota subscript)</td>
  </tr>
</table>

<p><strong>Note: </strong>some of the combining classes in this list do not currently have 
members but are specified here for completeness.</p>

<h3><a NAME="Decompositions and Normalization"></a>Decompositions and Normalization</h3>

<p>Decomposition is specified in Chapter three. The Unicode Technical Report #15 
Normalization Forms specifies the interaction between decomposition and normalization. The 
most up-to-date version is found on <a HREF="http://www.unicode.org/unicode/reports/tr15/">http://www.unicode.org/unicode/reports/tr15/</a>. 
That report specifies how the decompositions defined in the Unicode Character Database are 
used to derive normalized forms of Unicode text.</p>

<p>Note that as of the 2.1.9 update of the Unicode Character Database, the decompositions 
in the UnicodeData.txt file can be used to recursively derive the full decomposition in 
canonical order, without the need to separately apply canonical reordering. However, 
canonical reordering of combining character sequences must still be applied in 
decomposition when normalizing source text which contains any combining marks.</p>

<h3><a NAME="Case Mappings"></a>Case Mappings</h3>

<p>The case mapping is an informative, default mapping. Case itself, on the other hand, 
has normative status. Thus, for example, 0041 LATIN CAPITAL LETTER A is normatively 
uppercase, but its lowercase mapping the 0061 LATIN SMALL LETTER A is informative. The 
reason for this is that case can be considered to be an inherent property of a particular 
character (and is usually, but not always, derivable from the presence of the terms 
&quot;CAPITAL&quot; or &quot;SMALL&quot; in the character name), but case mappings between 
characters are occasionally influenced by local conventions. For example, certain 
languages, such as Turkish, German, French, or Greek may have small deviations from the 
default mappings listed in UnicodeData.</p>

<p>In addition to uppercase and lowercase, because of the inclusion of certain composite 
characters for compatibility, such as 01F1 LATIN CAPITAL LETTER DZ, there is a third case, 
called <i>titlecase</i>, which is used where the first letter of a word is to be 
capitalized (e.g. UPPERCASE, Titlecase, lowercase). An example of such a titlecase letter 
is 01F2 LATIN CAPITAL LETTER D WITH SMALL LETTER Z.</p>

<p>The uppercase, titlecase and lowercase fields are only included for characters that 
have a single corresponding character of that type. Composite characters (such as 
&quot;339D SQUARE CM&quot;) that do not have a single corresponding character of that type 
can be cased by decomposition.</p>

<p>For compatibility with existing parsers, UnicodeData only contains case mappings for 
characters where they are one-to-one mappings; it also omits information about 
context-sensitive case mappings. Information about these special cases can be found in a 
separate data file, <a HREF="ftp://ftp.unicode.org/Public/UNIDATA/SpecialCasing.txt">SpecialCasing.txt</a>, 
which has been added starting with the 2.1.8 update to the Unicode data files. 
SpecialCasing.txt contains additional informative case mappings that are either not 
one-to-one or which are context-sensitive.</p>

<h2><a NAME="Property Invariants"></a>Property Invariants</h2>

<p>Values in the Unicode Character Database are subject to correction as errors are found; 
however, some characteristics of the categories themselves can be considered invariants. 
Applications may wish to take these invariants into account when choosing how to implement 
character properties. The following is a partial list of known invariants for the Unicode 
Character Database.</p>

<h4>Database Fields</h4>

<ul>
  <li>The number of fields in the Unicode Character Database is fixed. </li>
  <li>The order of the fields is also fixed. <ul>
      <li>Any additional information about character properties to be added in the future will 
        appear in separate data tables, rather than being added on to the existing table or by 
        subdivision or reinterpretation of existing fields. </li>
    </ul>
  </li>
</ul>

<h4>General Category</h4>

<ul>
  <li>There will never be more than 32 General Category values. <ul>
      <li>It is very unlikely that the Unicode Technical Committee will subdivide the General 
        Category partition any further, since that can cause implementations to misbehave. Because 
        the General Category is limited to 32 values, 5 bits can be used to represent the 
        information, and a 32-bit integer can be used as a bitmask to represent arbitrary sets of 
        categories. </li>
    </ul>
  </li>
</ul>

<h4>Combining Classes</h4>

<ul>
  <li>Combining classes are limited to the values 0 to 255. <ul>
      <li>In practice, there are far fewer than 256 values used. Implementations may take 
        advantage of this fact for compression, since only the ordering of the non-zero values 
        matters for the Canonical Reordering Algorithm. It is possible for up to 256 values to be 
        used in the future; however, UTC decisions in the future may restrict the number of values 
        to 128, since this has implementation advantages. [Signed bytes can be used without 
        widening to ints in Java, for example.] </li>
    </ul>
  </li>
  <li>All characters other than those of General Category M* have the combining class 0. <ul>
      <li>Currently, all characters other than those of General Category Mn have the value 0. 
        However, some characters of General Category Me or Mc may be given non-zero values in the 
        future. </li>
      <li>The precise values above the value 0 are not invariant--only the relative ordering is 
        considered normative. For example, it is not guaranteed in future versions that the class 
        of U+05B4 will be precisely 14. </li>
    </ul>
  </li>
</ul>

<h4>Case</h4>

<ul>
  <li>Characters of type Lu, Lt, or Ll are called <i>cased</i>. All characters with an Upper, 
    Lower, or Titlecase mapping are cased characters. <ul>
      <li>However, characters with the General Categories of Lu, Ll, or Lt may not always have 
        case mappings, and case mappings may vary by locale. (See 
        ftp://ftp.unicode.org/Public/UNIDATA/SpecialCasing.txt). </li>
    </ul>
  </li>
</ul>

<h4>Canonical Decomposition</h4>

<ul>
  <li>Canonical mappings are always in canonical order. </li>
  <li>Canonical mappings have only the first of a pair possibly further decomposing. </li>
  <li>Canonical decompositions are &quot;transparent&quot; to other character data: <ul>
      <li><tt>BIDI(a) = BIDI(principal(canonicalDecomposition(a))</tt> </li>
      <li><tt>Category(a) = Category(principal(canonicalDecomposition(a))</tt> </li>
      <li><tt>CombiningClass(a) = CombiningClass(principal(canonicalDecomposition(a))</tt><br>
        where principal(a) is the first character not of type Mn, or the first character if all 
        characters are of type Mn. </li>
    </ul>
  </li>
  <li>However, because there are sometimes missing case pairs, and because of some legacy 
    characters, it is only generally true that: <ul>
      <li><tt>upper(canonicalDecomposition(a)) = canonicalDecomposition(upper(a))</tt> </li>
      <li><tt>lower(canonicalDecomposition(a)) = canonicalDecomposition(lower(a))</tt> </li>
      <li><tt>title(canonicalDecomposition(a)) = canonicalDecomposition(title(a))</tt> </li>
    </ul>
  </li>
</ul>

Source: https://unicode.org/

