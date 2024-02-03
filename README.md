```swift
  class MichalTalaga {
    var supportedLanguages = [".js", ".html", ".css", ".php", ".sql"]
    var supportedTools = ["WP", "Docker", "GIT", "CANVA", "FIGMA"]
    var isHired = false
    var age = 18.75
    var isAvailableForContact = true
    var email = "michal.talaga.programming@gmail.com"
    var currentProject = "Biblify"
    var futureSupportedTechnologies = ["Swift", "Sketch"]

    func introduce() -> String {
        let jobStatus = isHired ? "not looking for new
          opportunities" : "looking for new opportunities"
        return "👋 Hi there! I'm Michał Talaga, a dedicated developer.
          Currently \(jobStatus) at the age of \(age).
          Let's build something extraordinary together! 🚀"
    }

    func showcaseSkills() -> String {
        let languages = supportedLanguages.joined(separator: ", ")
        let tools = supportedTools.joined(separator: ", ")
        return "💻 My skills include: Languages - \(languages), Tools - \(tools)"
    }

    func currentProjectInfo() -> String {
        let projectInfo = currentProject != nil ? "🚧 Currently
          immersed in: \(currentProject!). Stay tuned for
          updates! ✨" : "🤔 Exploring new projects and
          challenges. Have a suggestion? Let me know!"
        return projectInfo
    }

    func futureSupportedTechnologiesInfo() -> String {
        let futureTechnologies = futureSupportedTechnologies.isEmpty ?
          "No specific plans for now" : "Exploring upcoming technologies
          like: \(futureSupportedTechnologies.joined(separator: ", ")) 🚀"
        return "🔮 \(futureTechnologies)"
    }

    func contactMe() -> String {
        var contactInfo = "📫 Feel free to reach out to me!"
        if let email = email {
            contactInfo += " You can contact me via email at \(email)."
        }
        contactInfo += isAvailableForContact ? " Let's connect and
          discuss exciting projects together." : " 🚧 Currently
          not available for direct contact, but keep an eye out
          for future updates!"
        return contactInfo
    }
}


```
