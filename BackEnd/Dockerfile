# Usa una imagen oficial de Tomcat como base
FROM tomcat:9.0

# Elimina la aplicación por defecto de Tomcat (opcional pero recomendable)
RUN rm -rf /usr/local/tomcat/webapps/*

# Copia tu fichero .war al directorio de despliegue de Tomcat
COPY DemoNetflix.war /usr/local/tomcat/webapps/ROOT.war

# Expon el puerto por donde corre Tomcat
EXPOSE 8080

# Comando para arrancar Tomcat
CMD ["catalina.sh", "run"]