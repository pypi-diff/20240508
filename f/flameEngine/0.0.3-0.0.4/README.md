# Comparing `tmp/flameengine-0.0.3.tar.gz` & `tmp/flameengine-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flameengine-0.0.3.tar", last modified: Mon May  6 15:08:15 2024, max compression
+gzip compressed data, was "flameengine-0.0.4.tar", last modified: Tue May  7 17:51:04 2024, max compression
```

## Comparing `flameengine-0.0.3.tar` & `flameengine-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 15:08:15.465275 flameengine-0.0.3/
--rw-rw-rw-   0        0        0      618 2024-05-06 15:08:15.464276 flameengine-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 15:08:15.457238 flameengine-0.0.3/flameEngine/
--rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.3/flameEngine/__init__.py
--rw-rw-rw-   0        0        0     1071 2024-05-06 15:01:26.000000 flameengine-0.0.3/flameEngine/example.py
--rw-rw-rw-   0        0        0    42987 2024-05-06 15:04:19.000000 flameengine-0.0.3/flameEngine/flame.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:08:15.462275 flameengine-0.0.3/flameEngine.egg-info/
--rw-rw-rw-   0        0        0      618 2024-05-06 15:08:15.000000 flameengine-0.0.3/flameEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-06 15:08:15.000000 flameengine-0.0.3/flameEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 15:08:15.000000 flameengine-0.0.3/flameEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-06 15:08:15.000000 flameengine-0.0.3/flameEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.3/license.txt
--rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 15:08:15.465275 flameengine-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      943 2024-05-06 15:07:35.000000 flameengine-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:51:04.005786 flameengine-0.0.4/
+-rw-rw-rw-   0        0        0      618 2024-05-07 17:51:04.004996 flameengine-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 17:51:03.998296 flameengine-0.0.4/flameEngine/
+-rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4/flameEngine/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4/flameEngine/example.py
+-rw-rw-rw-   0        0        0    43279 2024-05-07 17:16:46.000000 flameengine-0.0.4/flameEngine/flame.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:51:04.003276 flameengine-0.0.4/flameEngine.egg-info/
+-rw-rw-rw-   0        0        0      618 2024-05-07 17:51:03.000000 flameengine-0.0.4/flameEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-07 17:51:03.000000 flameengine-0.0.4/flameEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 17:51:03.000000 flameengine-0.0.4/flameEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 17:51:03.000000 flameengine-0.0.4/flameEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4/license.txt
+-rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 17:51:04.005786 flameengine-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      943 2024-05-07 17:50:59.000000 flameengine-0.0.4/setup.py
```

### Comparing `flameengine-0.0.3/PKG-INFO` & `flameengine-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.3
+Version: 0.0.4
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.3/flameEngine/example.py` & `flameengine-0.0.4/flameEngine/example.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 
 def simulate_flame(f, *args):
     f.simulate(*args)
 
 
 def main():
     tstart = time.time()
-    try:
-        set_start_method('spawn')  # Warning! ('spawn') must be called
-    except RuntimeError:
-        pass
+    # try:
+    #     set_start_method('spawn')  # Warning! ('spawn') must be called
+    # except RuntimeError:
+    #     pass
     # f1 = flame_sim(no_frames=1500)
     # f2 = flame_sim(no_frames=1500)
     #
     # t1 = Process(target=simulate_flame, args=(f1, 1, 0, 20, 0, 0, 0, 0, 0, 0, 0, 1, 1))
     # t2 = Process(target=simulate_flame, args=(f2, 0, 0, 20, 0, 0, 0, 0, 0, 0, 0, 1, 1))
     #
     # t1.start()
     # t2.start()
     #
     # t1.join()
     # t2.join()
-    f1 = flame_sim(no_frames=500,frame_skip=25)
-
-    f1.simulate( plot=0, save_animation=0, save_v=1, save_u=0, save_vu_mag=0, save_fuel=0,save_oxidizer=0,save_product=0, save_pressure=0, save_temperature=0, save_rgb=0, save_alpha=0)
+    f1 = flame_sim(no_frames=1000,frame_skip=25)
+    f1.simulate( plot=1, save_animation=0, save_v=0, save_u=0, save_vu_mag=0, save_fuel=0,save_oxidizer=0,save_product=0, save_pressure=0, save_temperature=0, save_rgb=0, save_alpha=0)
     tstop = time.time()
     total = tstop - tstart
     print(round(total, 2), '[s]')
 
 
 if __name__ == '__main__':
     # freeze_support()
```

### Comparing `flameengine-0.0.3/flameEngine/flame.py` & `flameengine-0.0.4/flameEngine/flame.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
                  th_point_c=273. + 400.,
                  d_low_product_r_c=1e-3,
                  d_high_product_r_c=1e1,
                  th_point_r_c=273. + 200.,
                  d_low_product_r_h=1e1,
                  d_high_product_r_h=20.,
                  th_point_r_h=273. + 400.):
-
         torch.cuda.synchronize()
         matplotlib.use('TkAgg')
         plt.style.use('dark_background')
         # CUDA_LAUNCH_BLOCKING = 1
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.no_frames = no_frames
         self.frame_skip = frame_skip
@@ -38,19 +37,25 @@
         self.grid_size_y = grid_y
         self.N_boundary = int(self.grid_size_x / 100)
         self.size_x = self.grid_size_x + self.N_boundary * 2
         self.size_y = self.grid_size_y + self.N_boundary * 2
         self.dx = 2 / (self.size_x - 1)  # [m]
         self.dy = 2 / (self.size_y - 1)
         self.dt = dt  # [s]
+        self.idy = None
+        self.idx = None
+        self.idy_v = None
+        self.idx_v = None
+        self.idy_u = None
+        self.idx_u = None
         self.degrees_of_freedom = 2
         self.viscosity = viscosity  # of air
         self.diff = diff
         self.avogardo = 6.022 * 10 * 1e23
-        self.gas_constant = R = 8.314
+        self.gas_constant = self.R = 8.314
         self.boltzmann_constant = 1.380649 * 10e-23
         self.gravity = 9.8
         self.gravity_divider = 2000
         self.propane_molecular_mass = 44.097 * 1e-3  # g/mol
         self.butane_molecular_mass = 58.12 * 1e-3  # g/mol
         self.oxygen_molecular_mass = 15.999 * 1e-3  # g/mol
         self.co2_molecular_mass = 44.01 * 1e-3  # g/mol
@@ -87,26 +92,25 @@
         self.d_low_product_r_h = d_low_product_r_h
         self.d_high_product_r_h = d_high_product_r_h
         self.th_point_r_h = th_point_r_h  # KELVINS
 
         self.low_alpha = 3.
         self.high_alpha = 12.
         self.alpha_decay = 0.001
-
         self.fuel_density = torch.zeros(self.size_x, self.size_y, device=self.device)
         self.fuel_density_prev = torch.zeros(self.size_x, self.size_y, device=self.device)
         self.oxidizer_density = torch.ones(self.size_x, self.size_y, device=self.device)
         self.oxidizer_density_prev = torch.ones(self.size_x, self.size_y, device=self.device)
         self.product_density = torch.zeros(self.size_x, self.size_y, device=self.device)
         self.product_density_prev = torch.zeros(self.size_x, self.size_y, device=self.device)
 
         self.u = torch.zeros(self.size_x, self.size_y, device=self.device)
         self.v = torch.zeros(self.size_x, self.size_y, device=self.device)
         self.velocity_magnitude = torch.zeros(self.size_x, self.size_y, device=self.device)
-
+        self.fuel_initial_speed = 5.
         # RANDOM WIND SPEEDS https://www.weather.gov/mfl/beaufort
         self.r1 = -0.1
         self.r2 = 0.1
         self.u_prev = torch.zeros((self.size_x, self.size_y), device=self.device)
         self.uniform_tensor = torch.zeros((self.grid_size_x - self.N_boundary - self.N_boundary,
                                            self.grid_size_y - self.N_boundary - self.N_boundary),
                                           device=self.device)
@@ -138,14 +142,41 @@
                                              device=self.device)  # m3
         self.mass_product_prev = torch.full((self.size_x, self.size_y), self.product_molecular_mass,
                                             device=self.device)  # m3
 
         self.alpha = torch.zeros_like(self.temperature, device=self.device)
         self.rgb = torch.zeros_like(torch.stack((self.temperature, self.temperature, self.temperature), dim=2))
 
+    def structure_example(self):
+        self.rg_u = 25
+        self.offset_vertical = int(self.grid_size_x / 3)
+        self.center_x = self.grid_size_x // 2
+        self.center_y = self.grid_size_y // 2
+        self.idx_x_low_u = self.center_x - self.rg_u + self.offset_vertical
+        self.idx_x_high_u = self.center_x + self.rg_u + self.offset_vertical
+        self.idx_y_low_u = self.center_y - self.rg_u
+        self.idx_y_high_u = self.center_y + self.rg_u
+        self.idx_u = slice(self.idx_x_low_u, self.idx_x_high_u)
+        self.idy_u = slice(self.idx_y_low_u, self.idx_y_high_u)
+
+        self.rg_v = 2
+        self.idx_x_low_v = self.center_x - self.rg_v + self.offset_vertical
+        self.idx_x_high_v = self.center_x + self.rg_v + self.offset_vertical
+        self.idx_y_low_v = self.center_y - self.rg_v
+        self.idx_y_high_v = self.center_y + self.rg_v
+        self.idx_v = slice(self.idx_x_low_v, self.idx_x_high_v)
+        self.idy_v = slice(self.idx_y_low_v, self.idx_y_high_v)
+
+        self.rg = 25
+        self.idx_x_low = self.center_x - self.rg + self.offset_vertical
+        self.idx_x_high = self.center_x + self.rg + self.offset_vertical
+        self.idx_y_low = self.center_y - self.rg-5
+        self.idx_y_high = self.center_y + self.rg+5
+        self.idx = slice(self.idx_x_low, self.idx_x_high)
+        self.idy = slice(self.idx_y_low, self.idx_y_high)
     @staticmethod
     def set_bnd(Nx, Ny, b, x):
         if b == 1:
             x[0, 1:Ny + 1] = 0.  # -x[1, 1:Ny + 1]
             x[Nx + 1, 1:Ny + 1] = 0.  # -x[Nx, 1:Ny + 1]
         else:
             x[0, 1:Ny + 1] = 0.  # x[1, 1:Ny + 1]
@@ -179,27 +210,19 @@
         denominator_mask = torch.abs(denominator) <= eps
         zero_mask = numerator_mask & denominator_mask
         result = torch.zeros_like(numerator, device=self.device)
         result[~zero_mask] = numerator[~zero_mask] / denominator[~zero_mask]
         return result
 
     def ignite(self, temperature, step):
-        rg = 25
-        offset_vertical = int(self.grid_size_x / 3)
-        center_x = self.grid_size_x // 2
-        center_y = self.grid_size_y // 2
-        idx_x_low = center_x - rg + offset_vertical
-        idx_x_high = center_x + rg + offset_vertical
-        idx_y_low = center_y - rg
-        idx_y_high = center_y + rg
         ignite_temp = 273. + 10300.  # Note: lighter temperature (273. + 1300.)
         if step > 75:
             pass
         else:
-            temperature[idx_x_low:idx_x_high, idx_y_low:idx_y_high] = ignite_temp
+            temperature[self.idx,self.idy] = ignite_temp
         return temperature
 
     def combustion(self, fuel_density, oxidizer_density, product_density,
                    u, v, temperature, step):
         temperature += self.ignite(temperature, step)
         density_treshold_unburned_fuel = ((fuel_density >= self.d_low_fuel) & (fuel_density <= self.d_high_fuel))
         density_treshold_unburned_oxizdizer = (
@@ -247,25 +270,23 @@
                                                                self.N_boundary:self.grid_size_y - self.N_boundary] * (
                                                                        horizontal_directivity.float()[
                                                                        self.N_boundary:self.grid_size_x - self.N_boundary,
                                                                        self.N_boundary:self.grid_size_y - self.N_boundary] * cooling_v_magnitude - cooling_v_magnitude / 2) * self.dt
         return u, v, oxidizer_density
 
     def radiative_cooling(self, fuel_density, oxidizer_density, product_density, u, v, temperature):
-
         density_treshold_burned_product = (
                 (product_density >= self.d_low_product_r_c) & (product_density <= self.d_high_product_r_c))
         above_temperature_treshold = (temperature >= self.th_point_r_c)
         conditions_met = density_treshold_burned_product & above_temperature_treshold
         u[conditions_met] += product_density[conditions_met] * (-u[conditions_met]) / 100
         v[conditions_met] += product_density[conditions_met] * (-v[conditions_met]) / 150
         return u, v, product_density
 
     def radiative_heating(self, fuel_density, oxidizer_density, product_density, u, v, temperature):
-
         density_treshold_burned_product = (
                 (product_density >= self.d_low_product_r_h) & (product_density <= self.d_high_product_r_h))
         above_temperature_treshold = (temperature >= self.th_point_r_h)
         conditions_met = density_treshold_burned_product & above_temperature_treshold
         u[conditions_met] += product_density[conditions_met] * (u[conditions_met]) / 250
         v[conditions_met] += product_density[conditions_met] * (v[conditions_met]) / 250
         return u, v, product_density
@@ -284,15 +305,14 @@
 
     def temperature2velocity(self, pressure, temperature, fuel_density, product_density, oxidizer_density,
                              mass_fuel, mass_oxidizer, mass_product,
                              degrees_of_freedom):
         kT = (self.boltzmann_constant * temperature)
         N_oxy_atoms = pressure * mass_oxidizer * self.grid_unit_volume / oxidizer_density / kT
         N_oxy_atoms = self.nan2zero(N_oxy_atoms, 0., 0., 0.)
-
         kinetic_energy_per_atom = (3 / degrees_of_freedom) * kT
         velocity_matrix_oxidizer = (2 * N_oxy_atoms * kinetic_energy_per_atom / mass_oxidizer) ** 0.5
         velocity_matrix_oxidizer = self.nan2zero(velocity_matrix_oxidizer, 0., 0., 0.)
         v = velocity_matrix_oxidizer - 2 * velocity_matrix_oxidizer * torch.rand(velocity_matrix_oxidizer.shape[0],
                                                                                  velocity_matrix_oxidizer.shape[1],
                                                                                  device=self.device)
 
@@ -340,29 +360,21 @@
         green[temperature < self.low_alpha] = 0
 
         return torch.clamp(torch.stack((red, green, blue), dim=2), 0, 255), self.alpha
 
     # w1(x) = w0(x) + dt * f(x,t)
     # Dynamic fuel_density addition
     def add_fuel_density(self, x, x0, dt, step):
-        rg = 25
-        offset_vertical = int(self.grid_size_x / 3)
-        center_x = self.grid_size_x // 2
-        center_y = self.grid_size_y // 2
-        idx_x_low = center_x - rg + offset_vertical
-        idx_x_high = center_x + rg + offset_vertical
-        idx_y_low = center_y - rg - 5
-        idx_y_high = center_y + rg + 5
-        idx_x = torch.randint(low=idx_x_low, high=idx_x_high, size=(1,))
-        idx_y = torch.randint(low=idx_y_low, high=idx_y_high, size=(1,))
-
-        x0[idx_x, idx_y] += (1.808 + 2.48)
-        x0[idx_x_low:idx_x_high, idx_y_low:idx_y_high] += (1.808 + 2.48)  # Note :  propane + butane kg/m3
-        x[idx_x_low:idx_x_high, idx_y_low:idx_y_high] += \
-            dt * x0[idx_x_low:idx_x_high, idx_y_low:idx_y_high]
+        # TODO: add fuel density with outside predefined fuel_density structure and behavior
+        if step < 500:
+            x0[self.idx,self.idy] += (1.808 + 2.48)  # Note :  propane + butane kg/m3
+            x[self.idx,self.idy] += \
+                dt * x0[self.idx,self.idy]
+        else:
+            pass
         return x, x0
 
     def add_oxidiser_density(self, x, x0, dt, step):
         # air density 1.225 kg/m3
         xmean = x0[self.N_boundary:self.grid_size_x - self.N_boundary,
                 self.N_boundary:self.grid_size_y - self.N_boundary].mean()
         # xx = torch.zeros_like(x0[N_boundary:grid_size_x, N_boundary:grid_size_y],device=device)
@@ -378,51 +390,36 @@
             self.N_boundary:self.grid_size_y - self.N_boundary] += dt * 1.225
         else:
             pass
         return x, x0
 
     # Static velocity field components
     def add_source_u(self, fuel_density, x, x0, dt, step):
-        rg = 25
-        offset_vertical = int(self.grid_size_x / 3)
-        center_x = self.grid_size_x // 2
-        center_y = self.grid_size_y // 2
-        idx_x_low = center_x - rg + offset_vertical
-        idx_x_high = center_x + rg + offset_vertical
-        idx_y_low = center_y - rg
-        idx_y_high = center_y + rg
-
-        fuel_speed = 5.
         # Fire
-        x0 -= fuel_speed * fuel_density
-
-        x[idx_x_low:idx_x_high, idx_y_low:idx_y_high] \
-            = dt * x0[idx_x_low:idx_x_high, idx_y_low:idx_y_high]
+        x0 -= self.fuel_initial_speed * fuel_density
+        x[self.idx_u,self.idy_u] \
+            = dt * x0[self.idx_u,self.idy_u]
 
         x[self.N_boundary:self.grid_size_x - self.N_boundary,
         self.N_boundary:self.grid_size_y - self.N_boundary] += dt * self.gravity / self.gravity_divider
 
         return x, x0
 
     def add_source_v(self, fuel_density, x, x0, dt, step):
-        rg = 2
-        offset_vertical = int(self.grid_size_x / 3)
-        center_x = self.grid_size_x // 2
-        center_y = self.grid_size_y // 2
-        idx_x_low = center_x - rg + offset_vertical
-        idx_x_high = center_x + rg + offset_vertical
-        idx_y_low = center_y - rg
-        idx_y_high = center_y + rg
-
         x0 += 2 * (torch.rand(x0.shape, device=self.device) - 0.5) * fuel_density
-
-        x[idx_x_low:idx_x_high, idx_y_low:idx_y_high] \
-            = dt * x0[idx_x_low:idx_x_high, idx_y_low:idx_y_high]
+        x[self.idx_v,self.idy_v] \
+            = dt * x0[self.idx_v,self.idy_v]
         return x, x0
 
+    def add_wind_u(self): # TODO: this
+        pass
+
+    def add_wind_v(self): # TODO: this
+        pass
+
     # Step 2
     # w2(x) = w1(p(x-dt))
     def advect(self, b, x, x0, u, v, dt):
         dt0 = dt * max(self.grid_size_x, self.grid_size_y)
         i, j = torch.meshgrid(torch.arange(1, self.grid_size_x, device=self.device),
                               torch.arange(1, self.grid_size_y, device=self.device),
                               indexing='ij')
@@ -483,15 +480,14 @@
         c = b + 1
         d = -b
         e = -c
         v_prev[b:d, b:d] = -0.5 * h * ((u[c:, b:d] - u[:e, b:d]) + (v[b:d, c:] - v[b:d, :e]))
         u_prev.fill_(0.)
         u_prev = self.set_bnd(self.grid_size_x, self.grid_size_y, 0, u_prev)
         v_prev = self.set_bnd(self.grid_size_x, self.grid_size_y, 0, v_prev)
-
         for k in range(20):
             u_prev[b:d, b:d] = (v_prev[b:d, b:d] + u_prev[:e, b:d] +
                                 u_prev[c:, b:d] + u_prev[b:d, :e] +
                                 u_prev[b:d, c:]) / 4.
             u_prev = self.set_bnd(self.grid_size_x, self.grid_size_y, 0, u_prev)
 
         u[b:d, b:d] = u[b:d, b:d] - 0.5 * (u_prev[c:, b:d] - u_prev[:e, b:d]) / h
@@ -645,15 +641,15 @@
             temperature, temperature_prev, \
             mass_fuel, mass_oxidizer, mass_product, \
             poisson_v_term, rgb, alpha
 
     def save_results(self, step, save_v=0, save_u=0, save_vu_mag=0, save_fuel=0, save_oxidizer=0,
                      save_product=0, save_pressure=0, save_temperature=0, save_rgb=0, save_alpha=0):
         if step % self.frame_skip == 0 or step == 0:
-            meta_data = torch.tensor([self.grid_size_x,self.grid_size_y,self.N_boundary,self.size_x,
+            meta_data = torch.tensor([step,self.fuel_initial_speed,self.grid_size_x,self.grid_size_y,self.N_boundary,self.size_x,
                           self.size_y,self.dx,self.dy,self.dt,self.degrees_of_freedom,
                           self.viscosity,self.diff,self.gravity,self.gravity_divider,
                           self.fuel_molecular_mass,self.oxidizer_molecular_mass,self.product_molecular_mass,
                           self.grid_unit_volume,self.d_low_fuel,self.d_high_fuel,self.d_low_oxidizer,
                           self.d_high_oxidizer,self.th_point_c,self.d_low_product_r_c,self.d_high_product_r_c,self.th_point_r_c,
                           self.d_low_product_r_h,self.d_high_product_r_h,self.th_point_r_h,self.low_alpha,self.high_alpha,self.alpha_decay])
             if save_v == 1:
@@ -714,15 +710,18 @@
                 my_folder = 'alpha'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.alpha}, f"{my_folder}/t{step}.pt")
             else:
                 pass
 
     def simulate(self, plot=0, save_animation=0, save_v=0, save_u=0, save_vu_mag=0, save_fuel=0,save_oxidizer=0,save_product=0, save_pressure=0, save_temperature=0, save_rgb=0, save_alpha=0):
-
+        if self.idx is None or self.idy is None:
+            self.structure_example()
+        else:
+            pass
         if plot == 1:
             # Create animation
             fig = plt.figure(figsize=(10, 6))
             grid = (2, 6)
             ax1 = plt.subplot2grid(grid, (0, 2))
             ax2 = plt.subplot2grid(grid, (0, 3))
             ax3 = plt.subplot2grid(grid, (0, 4))
@@ -779,18 +778,15 @@
                     temp = ax8.imshow((self.temperature.cpu().numpy()), cmap='plasma')
                     rgb = ax9.imshow((self.rgb.cpu().numpy()).astype(np.uint8), alpha=self.alpha.cpu().numpy())
                     ims.append(
                         [d, ox2, combustion_products, u_component, v_component, pressure_field, temp, vel_mag, rgb])
         if plot == 1:
             ani = animation.ArtistAnimation(fig, ims, interval=1, blit=True, repeat_delay=100)
         if save_animation == 1:
-            ani.save("fixed_alpha.gif")
+            ani.save("flame_animation.gif")
         if plot == 1:
             plt.show()
-
         torch.cuda.empty_cache()
         import sys
-
         sys.modules[__name__].__dict__.clear()
         import gc
-
         gc.collect()
```

### Comparing `flameengine-0.0.3/flameEngine.egg-info/PKG-INFO` & `flameengine-0.0.4/flameEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.3
+Version: 0.0.4
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.3/license.txt` & `flameengine-0.0.4/license.txt`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.3/setup.py` & `flameengine-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Flame simulation package'
 LONG_DESCRIPTION = 'Simulation engine implementation of stable fluids with extra steps for dataset generation in neural network env and test'
 
 setup(
     name="flameEngine",
     version=VERSION,
     author="Piotr Mikolajczyk",
```

