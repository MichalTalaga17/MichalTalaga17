```swift
  class MichalTalaga {
    var supportedLanguages: [String]
    var supportedTools: [String]
    var isHired: Bool
    var age: Double
    var favoriteEmojis: [String]
    var isAvailableForContact: Bool
    var email: String?
    var currentProject: String?
    var futureSupportedTechnologies: [String]

    init() {
        supportedLanguages = [".js", ".html", ".css", ".php", ".sql"]
        supportedTools = ["WP", "Docker", "GIT", "CANVA", "FIGMA"]
        isHired = false
        age = 18.75
        isAvailableForContact = true
        email = "michal.talaga.programming@gmail.com"
        currentProject = "Biblify"
        futureSupportedTechnologies = ["Swift", "Sketch"]
    }

    func introduce() -> String {
        return "👋 Hi there! I'm Michał Talaga,
          a dedicated developer with a passion for creating innovative solutions.
          Currently \(isHired ? "employed" : "looking for new opportunities") at the age of \(age).
          Let's build something extraordinary together! 🚀"
    }

    func showcaseSkills() -> String {
        let languages = supportedLanguages.joined(separator: ", ")
        let tools = supportedTools.joined(separator: ", ")
        return "💻 My skills include: Languages - \(languages), Tools - \(tools)"
    }

    func currentProjectInfo() -> String {
        if let project = currentProject {
            return "🚧 Currently immersed in: \(project). Stay tuned for updates! ✨"
        } else {
            return "🤔 Exploring new projects and challenges. Have a suggestion? Let me know!"
        }
    }

    func futureSupportedTechnologiesInfo() -> String {
        let futureTechnologies = futureSupportedTechnologies.isEmpty ? "No specific plans
          for now" : "Exploring upcoming technologies like: \(futureTechnologies.joined(separator: ", ")) 🚀"
        return "🔮 \(futureTechnologies)"
    }

    func contactMe() -> String {
        var contactInfo = "📫 Feel free to reach out to me!"
        if let email = email {
            contactInfo += " You can contact me via email at \(email)."
        }
        contactInfo += isAvailableForContact ? " Let's connect and discuss exciting projects together." :
          " 🚧 Currently not available for direct contact, but keep an eye out for future updates!"
        return contactInfo
    }
}

```
