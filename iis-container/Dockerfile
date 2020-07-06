FROM mcr.microsoft.com/windows/servercore/iis:windowsservercore-ltsc2019

RUN powershell.exe -Command \
  Set-ExecutionPolicy Bypass -Scope Process ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-WebServerRole ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-WebServer ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-CommonHttpFeatures ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-HttpErrors ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-HttpRedirect ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-ApplicationDevelopment ; \
  Enable-WindowsOptionalFeature -online -FeatureName NetFx4Extended-ASPNET45 ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-NetFxExtensibility45 ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-HealthAndDiagnostics ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-HttpLogging ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-LoggingLibraries ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-RequestMonitor ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-HttpTracing ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-Security ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-RequestFiltering ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-Performance ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-Security ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-BasicAuthentication ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-WindowsAuthentication ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-StaticContent ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-DefaultDocument ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-WebSockets ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-ApplicationInit ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-ISAPIExtensions ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-ISAPIFilter ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-HttpCompressionStatic ; \
  Enable-WindowsOptionalFeature -Online -FeatureName IIS-ASPNET45

WORKDIR c:/inetpub/wwwroot

EXPOSE 80 443