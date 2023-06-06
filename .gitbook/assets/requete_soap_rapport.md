<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:edit="http://suravenir.fr/ws/odet/services/edition">
    <soapenv:Header/>
    <soapenv:Body>
        <edit:startEdition>
            <!--  Optional:  -->
            <edition>
                <cdDivFrmJuridique>DATA</cdDivFrmJuridique>
                <!--  Optional:  -->
                <cdEfs>DATA</cdEfs>
                <!--  Optional:  -->
                <cdProduit>DATA</cdProduit>
                <!--  Optional:  -->
                <cdSgnElec>DATA</cdSgnElec>
                <!--  Optional:  -->
                <cdSubDivFrmJuridique>DATA</cdSubDivFrmJuridique>
                <fluxXmlDemandeEdition>
                <![CDATA[ <!-- DATA --> ]]>
                </fluxXmlDemandeEdition>
                <!--  Optional:  -->
                <idLiasse>DATA</idLiasse>
                <!--  Zero or more repetitions:  -->
                <noPartenaire>DATA</noPartenaire>
                <!--  Optional:  -->
                <noPersonne>DATA</noPersonne>
                <!--  Optional:  -->
                <noPolice>DATA</noPolice>
                <!--  Optional:  -->
                <noSalarie>DATA</noSalarie>
                <!--  Optional:  -->
                <noStructure>DATA</noStructure>
                <previsualisation>DATA</previsualisation>
                <recu>DATA</recu>
            </edition>
        </edit:startEdition>
    </soapenv:Body>
</soapenv:Envelope>