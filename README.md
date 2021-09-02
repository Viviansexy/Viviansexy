- 👋 Hi, I’m @Viviansexy
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Viviansexy/Viviansexy is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
public static final boolean a(Activity var0, boolean var1) {
      if (a()) {
         var0.startActivity(new Intent(var0, SplashActivity.class));
         var0.finish();
         return false;
      } else {
         Intent var2 = var0.getIntent();
         boolean var3;
         if (var2 != null && (1048576 & var2.getFlags()) == 1048576) {
            var3 = true;
         } else {
            var3 = false;
         }

         if (var3) {
            var0.getClass().getSimpleName();
            var0.startActivity(new Intent(var0, SplashActivity.class));
            var0.finish();
            return false;
         } else {
            var0.getClass().getSimpleName();
            String var5 = var0.getComponentName().getClassName();
            String var6 = LauncherActivity.class.getPackage().getName();
            String var7 = RegisterIdentityCredentialLauncherActivity.class.getPackage().getName();
            if (!(var0 instanceof SplashActivity) && !var5.startsWith(var6) && !var5.startsWith(var7) && !var1) {
               a0 var11 = i0.a.a.a.a2.d.d();
               if (var11 == null || var11.l() == null) {
                  String var12 = var0.getPackageName();
                  Intent var13 = var0.getPackageManager().getLaunchIntentForPackage(var12);
                  if (var13 == null) {
                     return false;
                  }

                  var13.addFlags(67108864);
                  var0.startActivity(var13);
                  var0.finish();
                  return false;
               }
            }

            label40: {
               if (i0.a.a.a.h.u.b.c.a(i0.a.a.a.h.u.b.a.SHOW_EU_TOS) && !var5.startsWith(var6)) {
                  if (!(var0 instanceof SettingsBaseFragmentActivity)) {
                     break label40;
                  }

                  int var10 = ((SettingsBaseFragmentActivity)var0).h;
                  if (var10 != 11 && var10 != 19) {
                     break label40;
                  }
               }

               LayoutParams var8 = var0.getWindow().getAttributes();
               var0.getWindow().setSoftInputMode(3 | var8.softInputMode);
               var0.requestWindowFeature(1);
               return true;
            }

            var0.startActivity(ConfirmUpgradeTosActivity.a(var0));
            var0.finish();
            return false;
         }
      }
   }

   public static final void b(Activity var0) {
      var0.getClass().getSimpleName();
