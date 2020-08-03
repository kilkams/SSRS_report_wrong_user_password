# SSRS_report_wrong_user_password for SSRS

0. You need to add the linked server ADSI to the root of the forest 
1. Replace LDAP://controller-01.domain.corp and LDAP://controller-02.domain.corp and LDAP://controller-03.domain.corp and LDAP://controller-04.domain.corp and LDAP://controller-05.domain.corp to your FQDN name.
2. Replace <Value>subdomain1</Value> and <Value>subdomain2</Value> to your subdomain name
3. Replace <ParameterValue>
            <Value>domain</Value>
            <Label>domain</Label>
          </ParameterValue> to your domain name
4. Replace   <rd:ReportServerUrl>http://mssql.domain.corp/ReportServer</rd:ReportServerUrl> to your report server URL

Some field is not replicated between domain controllers, so data must be taken from all controllers separately
