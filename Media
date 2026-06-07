import android.content.Context
import android.content.Intent

fun sharePlantToSocialMedia(context: Context, plantName: String, scientificName: String, wateringDays: Int) {
    val shareBody = """
        🌿 Check out my latest garden species!
        
        Name: $plantName ($scientificName)
        Watering Schedule: Every $wateringDays days
        
        Cataloged with Gardening Assistant 🌸
    """.trimIndent()

    val intent = Intent(Intent.ACTION_SEND).apply {
        type = "text/plain"
        putExtra(Intent.EXTRA_SUBJECT, "My Green Companions")
        putExtra(Intent.EXTRA_TEXT, shareBody)
    }
    
    context.startActivity(Intent.createChooser(intent, "Share Plant Profile via"))
}
