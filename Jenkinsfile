node {
    def serviceName = "sampleapp"
    def prodIp = "10.100.192.200"
    def proxyIp = "10.100.192.200"
    def registryIpPort = "10.100.198.200:5000"
    def instances = 1

    def flow = load "/var/jenkins_home/scripts/utils.groovy"

    git url: "https://github.com/shrekze/samplewebapp.git"
    
    flow.provision(sampleapp)
    flow.buildService(serviceName, registryIpPort)
}
