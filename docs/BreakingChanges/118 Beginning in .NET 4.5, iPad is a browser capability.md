## 118: Beginning in .NET 4.5, iPad is an identifier in the default ASP.NET browser capabilities file, so it should not be used in a custom capabilties file

### Scope
Edge

### Version Introduced
4.5

### Change Description
Beginning in .NET 4.5, iPad is an identifier in the default ASP.NET browser capabilities file, so it should not be used in a custom capabilties file

- [ ] Quirked
- [ ] Build-time break
- [x] Source analyzer planned

### Recommended Action
If iPad-specific capabilities are required, it is necessary to modify iPad behavior by setting capabilities on the pre-defined gateway refID "IPad" instead of by generating a new "IPad" ID by user agent matching.

### Affected APIs
* Not detectable via API analysis

<!--
    ### Notes
    For analyzer, can look for 'iPad' in .browser capability files
-->
