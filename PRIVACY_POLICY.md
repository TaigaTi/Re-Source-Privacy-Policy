# Privacy Policy for Re-Source

**Last Updated: December 15, 2024**

Thank you for using Re-Source! This Privacy Policy explains how we collect, use, store, and protect your information when you use the Re-Source mobile application.

## 1. Information We Collect

### 1.1 Personal Information
When you use Re-Source, we collect the following personal information:
- **Email Address**: Used for account creation and authentication
- **User ID**: A unique identifier (Firebase UID) assigned to your account
- **Password**: Securely managed by Firebase Authentication (we never store your plain-text password)
- **Profile Images**: Optional images you upload for your user profile

### 1.2 User-Generated Content
We collect and store the content you create within the app:
- **Categories**: Names, colors, timestamps (created and last accessed)
- **Resources/Links**: URLs, titles, descriptions, images, timestamps (added and last accessed)
- **Metadata**: Information about your saved links including ownership data

### 1.3 Automatically Collected Information
- **Crash Reports and Analytics**: We use Firebase Crashlytics to collect information about app crashes and errors to improve app stability and performance
- **Usage Data**: Timestamps of when content is created and accessed

## 2. How We Use Your Information

We use the collected information for the following purposes:
- **Account Management**: To create, maintain, and authenticate your user account
- **Service Delivery**: To provide the core functionality of saving, organizing, and managing your resources
- **App Improvement**: To identify and fix bugs, crashes, and performance issues
- **Data Synchronization**: To sync your data across devices using the same account

## 3. Data Storage

### 3.1 Cloud Storage (Firebase)
**Re-Source stores all user data in the cloud using Google Firebase services.** Your data is NOT stored locally on your device. Specifically:

- **Firebase Authentication**: Manages your email/password login credentials
- **Cloud Firestore**: Stores all your user data including:
  - User profile information (email, profile image URLs)
  - All categories you create
  - All resources/links you save with their associated metadata
- **Firebase Storage**: Stores uploaded images including:
  - Profile pictures
  - Resource/link preview images

### 3.2 Data Structure
Your data in Firebase is organized as follows:
```
users/{userId}/
  - email
  - profileImageUrl
  - profileImageStoragePath
  - categories/{categoryId}/
      - name
      - color
      - createdAt
      - lastAccessed
      - resources/{resourceId}/
          - title
          - link
          - description
          - image
          - storagePath
          - addedAt
          - lastAccessed
          - ownerId
```

### 3.3 Security Measures
Firebase provides enterprise-grade security for your data:
- **Encryption in Transit**: All data transmitted between your device and Firebase servers is encrypted using HTTPS/TLS
- **Encryption at Rest**: Data stored in Firebase is encrypted at rest
- **Authentication**: Firebase Authentication ensures only you can access your account
- **Access Control**: Firebase Security Rules restrict data access to authenticated users and their own data
- **Compliance**: Firebase complies with major security certifications including SOC 2, ISO 27001, and others

## 4. Third-Party Services and Data Processors

### 4.1 Google/Firebase Services
Re-Source uses the following Google Firebase services, making Google a data processor for Re-Source:
- **Firebase Authentication**: For user account management
- **Cloud Firestore**: For database storage
- **Firebase Storage**: For image storage
- **Firebase Crashlytics**: For crash reporting and analytics

Google Firebase's privacy practices are governed by their privacy policy, which you can review at: https://firebase.google.com/support/privacy

### 4.2 Google's Role
Google Firebase acts as a service provider and data processor on behalf of Re-Source. Google processes your data according to their terms of service and privacy policies, and maintains certifications for data security and privacy compliance.

## 5. Third-Party Websites and HTTP Requests

### 5.1 Metadata Fetching
When you save a URL/link in Re-Source, the app:
- Makes a **direct HTTP request** to the provided URL from your device
- Parses the webpage HTML to extract metadata including:
  - Open Graph tags (og:title, og:description, og:image)
  - Standard meta tags (description, title)
  - Page title and preview images
- **Does NOT use a proxy server** - your device connects directly to the target website

### 5.2 Privacy Implications
When fetching metadata:
- The target website may log your IP address and device information
- The target website's privacy policy applies to this interaction
- Re-Source does not control or have visibility into what data third-party websites collect

## 6. Data Sharing

We do not sell, rent, or share your personal information with third parties except:
- **With your consent**: When you explicitly authorize data sharing
- **Service Providers**: With Google Firebase as described in Section 4
- **Legal Requirements**: When required by law, regulation, legal process, or governmental request
- **Safety and Security**: To protect the rights, property, or safety of Re-Source, our users, or the public

## 7. Data Location and Infrastructure

### 7.1 Firebase Infrastructure
Your data is stored on Google Firebase's cloud infrastructure. Firebase operates data centers in multiple regions worldwide, and your data may be stored and processed in any of these locations based on Google's infrastructure configuration.

### 7.2 International Data Transfers
By using Re-Source, you consent to your data being transferred to and processed in countries where Google Firebase operates, which may have different data protection laws than your country of residence.

## 8. Your Rights and Choices

### 8.1 Access and Control
You have the following rights regarding your data:
- **Access**: You can view all your data within the Re-Source app
- **Modification**: You can edit your profile, categories, and resources at any time
- **Deletion**: You can delete individual resources, categories, or your entire account

### 8.2 Account Deletion
When you delete your Re-Source account:
- Your user profile is permanently deleted from Firestore
- All your categories and resources are permanently deleted from Firestore
- Your authentication account is deleted from Firebase Auth
- Profile images and resource images are deleted from Firebase Storage
- **Note**: This deletion is permanent and cannot be undone

### 8.3 Data Export
Currently, Re-Source does not provide an automated data export feature. If you wish to export your data before deletion, please contact us at the email provided in Section 12.

### 8.4 App Uninstallation
**Important**: Simply uninstalling the Re-Source app does NOT delete your cloud-stored data. Your data remains in Firebase and will be available if you reinstall the app and log in again. To permanently delete your data, you must delete your account from within the app before uninstalling.

## 9. Data Retention

### 9.1 Active Accounts
We retain your data for as long as your account is active or as needed to provide you services.

### 9.2 Deleted Accounts
When you delete your account, your data is immediately removed from our active databases. However:
- Some data may remain in backup systems for a limited period according to Firebase's backup policies
- Firebase may retain certain data according to their data retention policies
- Crash logs and analytics data may be retained temporarily according to Firebase Crashlytics retention policies

### 9.3 Inactive Accounts
We do not automatically delete inactive accounts. Your data will remain in Firebase until you delete your account.

## 10. Children's Privacy

Re-Source is not intended for use by children under the age of 13. We do not knowingly collect personal information from children under 13. If we discover that we have collected personal information from a child under 13, we will delete that information immediately. If you believe we have collected information from a child under 13, please contact us at the email provided in Section 12.

## 11. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in our practices or for legal, regulatory, or operational reasons. When we make changes:
- We will update the "Last Updated" date at the top of this policy
- For significant changes, we may notify you through the app or via email
- Your continued use of Re-Source after changes are posted constitutes acceptance of the updated policy

We encourage you to review this Privacy Policy periodically to stay informed about how we protect your information.

## 12. Contact Information

If you have any questions, concerns, or requests regarding this Privacy Policy or how we handle your data, please contact us at:

**Email**: support@re-source.app

For issues specifically related to Firebase/Google services and data processing, you may also refer to:
- Firebase Privacy Policy: https://firebase.google.com/support/privacy
- Google Privacy Policy: https://policies.google.com/privacy

---

## Summary

**Key Points to Remember:**
- ✓ Re-Source stores ALL data in the cloud using Google Firebase (not locally on your device)
- ✓ We collect your email, user ID, and any content you create
- ✓ Google Firebase acts as our service provider and processes your data
- ✓ When you save links, your device makes direct HTTP requests to those websites
- ✓ Uninstalling the app does NOT delete your data - you must delete your account
- ✓ Firebase provides enterprise-grade security with encryption in transit and at rest
- ✓ You can delete your account and all data at any time from within the app

By using Re-Source, you acknowledge that you have read and understood this Privacy Policy and agree to its terms.
