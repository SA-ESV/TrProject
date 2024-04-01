<?xml version="1.0"?>
<Client>
	<FirstName>Ivan</FirstName>
	<SecondName>Ivanovich</SecondName>
	<LastName>Ivanov</LastName>
	<ContactNo>1234567890</ContactNo>
	<Email>III_780229@test.tst</Email>
	<BirthDate>29/02/1978</BirthDate>
	<Address>
		<City>Omsk</City>
		<Street>Sovetskaya</Street>
		<Zip>111111</Zip>
	</Address>
	<Status>Active</Status>
</Client>


<?xml version="1.0" encoding="utf-8"?>
<!-- Created with Liquid Technologies Online Tools 1.0 (https://www.liquid-technologies.com) -->
<xs:schema attributeFormDefault="unqualified" elementFormDefault="qualified" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:element name="Client">
    <xs:complexType>
      <xs:sequence>
        <xs:element name="FirstName" type="xs:string" />
        <xs:element name="SecondName" type="xs:string" />
        <xs:element name="LastName" type="xs:string" />
        <xs:element name="ContactNo" type="xs:unsignedInt" />
        <xs:element name="Email" type="xs:string" />
        <xs:element name="BirthDate" type="xs:string" />
        <xs:element name="Address">
          <xs:complexType>
            <xs:sequence>
              <xs:element name="City" type="xs:string" />
              <xs:element name="Street" type="xs:string" />
              <xs:element name="Zip" type="xs:unsignedInt" />
            </xs:sequence>
          </xs:complexType>
        </xs:element>
        <xs:element name="Status" type="xs:string" />
      </xs:sequence>
    </xs:complexType>
  </xs:element>
</xs:schema>