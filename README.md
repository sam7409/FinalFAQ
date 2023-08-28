# SupportDocs: DataSource
This branch is where SupportDocs gets its data! You can add, edit, and delete documents here. For usage instructions, check out the `README`'s [usage](https://github.com/aheze/SupportDocs#using-the-github-repository) section in the main branch.

## Data Source JSON URL
<a href="https://raw.githubusercontent.com/sam7409/FinalFAQ/DataSource/_data/supportdocs_datasource.json">https://raw.githubusercontent.com/sam7409/FinalFAQ/DataSource/_data/supportdocs_datasource.json</a>

<details markdown="1">
<summary><strong>Show examples</strong></summary>

<hr>

### SwiftUI
```swift
struct SwiftUIExampleView_MinimalCode: View {
    let dataSource = URL(string: "https://raw.githubusercontent.com/sam7409/FinalFAQ/DataSource/_data/supportdocs_datasource.json")!
    @State var supportDocsPresented = false
    
    var body: some View {
        Button("Present SupportDocs from SwiftUI!") { supportDocsPresented = true }
        .sheet(isPresented: $supportDocsPresented, content: {
            SupportDocsView(dataSource: dataSource, isPresented: $supportDocsPresented)
        })
    }
}
```

### UIKit
```swift
class UIKitExampleController_MinimalCode: UIViewController {
    /**
    Connect this inside the storyboard.
    
    This is just for demo purposes, so it's not connected yet.
    */
    @IBAction func presentButtonPressed(_ sender: Any) {
        let dataSource = URL(string: "https://raw.githubusercontent.com/sam7409/FinalFAQ/DataSource/_data/supportdocs_datasource.json")!
    
        let supportDocsViewController = SupportDocsViewController(dataSource: dataSource)
        self.present(supportDocsViewController, animated: true, completion: nil)
    }
}
```

<hr>

</details>

## Table of Contents
- [404 Page](https://sam7409.github.io/FinalFAQ/404) (SupportDocs Integrated File) ([edit](https://github.com/sam7409/FinalFAQ/edit/DataSource/FinalFAQ/404.md))
- [Can I access my subscription from another device?](https://sam7409.github.io/FinalFAQ/QNAFive/AccessSubscriptionFromOtherDevice) (Can I access my subscription from another device?) ([edit](https://github.com/sam7409/FinalFAQ/edit/DataSource/QNAFive/AccessSubscriptionFromOtherDevice.md))
- [Can I transfer my subscription to another Apple ID?](https://sam7409.github.io/FinalFAQ/QNASix/TransferSubscriptionToAnotherAppleID) (Can I transfer my subscription to another Apple ID?) ([edit](https://github.com/sam7409/FinalFAQ/edit/DataSource/QNASix/TransferSubscriptionToAnotherAppleID.md))
- [How can I restore my subscription?](https://sam7409.github.io/FinalFAQ/QNAFour/RestoreMyProSubscription) (How can I restore my subscription?) ([edit](https://github.com/sam7409/FinalFAQ/edit/DataSource/QNAFour/RestoreMyProSubscription.md))
- [How to cancel subscription?](https://sam7409.github.io/FinalFAQ/QNATWO/HowToCancelProSubscription) (How to cancel subscription?) ([edit](https://github.com/sam7409/FinalFAQ/edit/DataSource/QNATWO/HowToCancelProSubscription.md))
- [How to get refund?](https://sam7409.github.io/FinalFAQ/QNAThree/HowToGetRefund) (How to get refund?) ([edit](https://github.com/sam7409/FinalFAQ/edit/DataSource/QNAThree/HowToGetRefund.md))
- [How to switch subscription plan ?](https://sam7409.github.io/FinalFAQ/QNAONE/HowToChangeSubscription) (How to switch subscription plan ?) ([edit](https://github.com/sam7409/FinalFAQ/edit/DataSource/QNAONE/HowToChangeSubscription.md))


## Notes
- Your changes make take up to five minutes to deploy. You can track the deployment progress [here](https://github.com/sam7409/FinalFAQ/deployments/activity_log?environment=github-pages).
- Do **not** update this file (`README.md`) directly. Your changes will be overriden the next time you push (the GitHub Action will regenerate this file). Instead, update the file in [`_scripts/README.md`](https://github.com/sam7409/FinalFAQ/edit/DataSource/_scripts/README.md). 