# TODO: Implement Client Base Tab

## Steps to Complete

1. **Modify Address Model**  
   - Update `models.py`: Replace `address_text` with structured fields: `postal_code` (CharField, max_length=6), `region`, `city`, `street`, `house_number`, `building`, `office_number`.

2. **Create Migration**  
   - Run `python manage.py makemigrations` to generate migration for Address model changes.

3. **Update add_address View**  
   - Modify `add_address` function in `views.py` to handle new structured fields.

4. **Update Forms and Templates**  
   - Update `add_address_form.html` to include fields for the new address structure.

5. **Add Client Base View**  
   - Create `client_base_view` in `views.py` to list unique organizations with their legal and actual addresses.

6. **Add URL**  
   - Add path for client_base in `urls.py`.

7. **Create Template**  
   - Create `client_base.html` template in `templates/requests/` to display the client base list.

8. **Update Home Template**  
   - Add link to client base in `home.html`.

9. **Run Migrations**  
   - Execute `python manage.py migrate` to apply database changes.

10. **Test Functionality**  
    - Verify the client base tab works correctly, including adding addresses and viewing the list.
